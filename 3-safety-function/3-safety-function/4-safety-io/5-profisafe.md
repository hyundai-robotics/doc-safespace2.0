<script id="page-config" type="application/json">
{
	"permittedStrs": ["HI6"]
}
</script>


# 3.3.4.5 PROFIsafe

### 1) PROFIsafe?
- 一种在 PROFINET/PROFIBUS 上运行的安全协议（安全配置）。
- 通过标准的 PROFINET 通信通道（“黑色通道”）传输安全数据。
- 支持无需额外接线的安全信号传输。

### 2) PROFINET & PROFIsafe 规范
- 数字输入：50、120 或 240 字节（选择一个）
- 数字输出：50、120 或 240 字节（选择一个）
- 安全 I/O：8/8 字节（启用或禁用）
- 最小通信周期：1 毫秒
- 支持的通信速度：10 或 100 Mbps
- 符合性等级：B
- 网络负载类别：II
- 可选功能：遗留、MRP

### 3) PROFIsafe 参数

`[System > 2: Control Parameters > 11: Industrial Communication > 6: Safety Communication > 2: PROFIsafe]`<br>
![](../../../_assets/safetyio_profisafe/profisafe_param.png)

 - 源地址：设置源地址。（固定为 1）
 - 目标地址：设置目标地址。（设置范围：1 到 65534）
 
 ***注意***<br> 
 - 地址类型：地址类型 1（仅允许目标地址）
 - 设备故障时的反应：如果该设备进入故障状态，所有 F-输出将变为安全状态（0）。一旦设备的故障状态得到解决，需要使用 F-主机的 Global-Acknowledge 等命令重新集成 F-设备。
 

### 4) PROFIsafe 配置过程

1) BD671 与 F-Host 和 Hi7 Com 之间的连接
2) GSDML 文件注册（TIA Portal）
3) PROFIsafe 控制器配置（TIA Portal）
<br>3.1) PROFINET 配置
<br>3.2) PROFIsafe 配置
4) Hi7 配置（TP UI）
<br>4.1) PROFINET 配置
<br>4.2) PROFIsafe 配置
5) 验证 PROFINET 和 PROFIsafe 通信
6) PROFINET I/O 信号的分配（FB 块设置）
7) PROFIsafe I/O 信号的分配


#### 4.1) BD671 与 F-Host 和 Hi7 Com 之间的连接

##### 4.1.1) LAN 电缆连接
1) 使用 LAN 电缆连接“PROFIsafe F-Host”和 BD671。
2) 验证链接 LED 是否闪烁。
3) 使用 LAN 电缆连接 Hi7 COM 的 LAN3 连接器与 BD671。
4) 验证链接 LED 是否闪烁。

![](../../../_assets/safetyio_profisafe/profisafe_connect.png)

##### 4.1.2) Hi7 Com 连接设置
1) 导航到以下菜单： **System -> Control Parameters -> Industrial Communication -> EtherCAT Master Settings**
2) 配置设置如下：
- EtherCAT 主站：开启
- 端口：LAN3
3) 从从站列表中选择“OptionBD - PROFINET_IO”，并按下 **Apply** 按钮。
4) 重启 Hi7 机器人控制器。
5) 重启后，检查 **Run**、**Communication** 和 **Error** LED 的状态。

![](../../../_assets/safetyio_profisafe/EC_master_setting1.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/EC_master_setting2.png)


#### 4.2) GSDML 文件注册（TIA Portal）
1) 启动 TIA Portal。
2) 导航到右侧菜单： **[Options] → [Manage general station description file (GSD)]**。
3) 点击 **"..."** 按钮并选择 GSDML 文件所在的目录。
4) 从屏幕上显示的列表中选择 **"GSDML-V2.43-Hyundai-Robotics-HI6-20251127.xml"** 并点击 **[Install]** 按钮。
5) 验证该文件是否已在硬件目录中注册为新设备。 <br>
![](../../../_assets/safetyio_profisafe/profisafe_gsdmal.png)

#### 4.3) PROFIsafe 控制器配置（TIA Portal）
##### 4.3.1) PROFINET 配置
1) 启动 TIA Portal 并创建一个新项目。
2) 双击 **Devices & Networks** 以打开它。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network.png)

3) 选择支持 PROFIsafe 通信的控制器（例如，CPU 1511F-1 PN）并将其拖入 **Network View**。
4) 从硬件目录中选择上一步中添加的设备（HRC, PROFINET I/O DAP），并将其拖入 **Network View**。
5) 在图中通过拖放连接两个设备之间的 LAN 端口。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network2.png)

6) 双击 **"Devices & Networks"** 视图中的 HRC-IO 设备。
7) 选择所需的插槽。
8) 从右侧目录中拖动所需模块（DI、DO 或 PROFIsafe I/O），并放入 **"Device Overview"** 窗口中。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network3.png)

9) 双击 **"Devices & Networks"** 视图中的 HRC-IO 设备。
10) 再次点击 HRC-IO 设备以打开 **Properties**（设置）窗口。
11) 转到底部的 **General** 标签。
12) 从左侧菜单中选择 **Ethernet addresses**。
13) 取消选择 **"Generate PROFINET device name automatically"** 选项。
14) 将 **"PROFINET device name"** 设置为 **"hd-hrc-hi7"** 并保存更改。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network4.png)

##### 4.3.2) PROFIsafe 配置
1) 双击 **"Devices & Networks"** 视图中的 HRC-IO 设备。
2) 在右侧的 **"Device Overview"** 窗口中选择 PROFIsafe 插槽。
3) PROFIsafe 通信设置将出现在底部窗格中。
4) 点击 **PROFIsafe** 标签。
5) 将 **F_Dest_Add** 设置为 1。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network5.png)

#### 4.4) Hi7 配置（TP UI）
##### 4.4.1) PROFINET 配置
1) 使用与 F-Host 中设置的相同值配置参数：
- PROFINET IO 设备名称：hd-hrc-hi7
- 插槽 1：数字输入：240
- 插槽 2：数字输出：240
- 插槽 3：安全 I/O：选择
2) 按下 **"Apply"** 按钮。<br>
![](../../../_assets/safetyio_profisafe/4_1_profinet_config.png)

##### 4.4.2) PROFIsafe 配置

1) 将 **目标地址** 设置为 1，使用在上一部分中配置的相同值。
2) 按下 **"Apply"** 按钮。<br>
![](../../../_assets/safetyio_profisafe/4_2_profisafe_config.png)

#### 4.5) 验证 PROFINET 和 PROFIsafe 通信

#### 4.5.1) 安全梯形图程序（TIA Portal）
1) 在 **Device Overview** 标签中，创建如下所示的梯形图程序并下载到控制器中。<br>
![](../../../_assets/safetyio_profisafe/5_1_Safety_Ladder.png)
2) 下载后，验证 **Distributed I/O** 屏幕上是否显示绿色勾选框。<br>
![](../../../_assets/safetyio_profisafe/5_1_Safety_Ladder2.png)

#### 4.5.2) TP 屏幕
1) PROFINET <br>
从菜单中导航到 **System -> 2: Control Parameters -> 11: Industrial Communication -> 5: PROFINET Settings**。<br>
![](../../../_assets/safetyio_profisafe/5_2_pnio_status.png)
- 检查每个插槽的状态信息。
- 验证计数器是否持续增加。

2) PROFIsafe <br>
从菜单中导航到 **System > 2: Control Parameters > 11: Industrial Communication > 6: Safety Communication > 2: PROFIsafe**。<br>
![](../../../_assets/safetyio_profisafe/5_2_profisafe_status.png)
- 验证 **FappState** 设置为 **CYCLE Data EX**。
- 验证 **Counter** 是否持续增加。

#### 4.6) PROFINET I/O 信号的分配（FB 块设置）
1) 导航到 **System → Control Parameters → I/O Signal Settings → FB Block Assignment**。
2) 根据需要将块设置更改为 **PROFINET I/O**，最多可设置 2 个块。
 （最大 PROFINET I/O 大小为 240 字节，每个单独 FB 块大小为 120 字节。因此，**超过 2 个块的任何设置将被忽略。**）<br>
![](../../../_assets/safetyio_profisafe/6_fb_block.png)

3) 此外，导航到 **Condition Settings** 菜单，确认 **PLC 操作模式** 设置为 **OFF**。<br>
![](../../../_assets/safetyio_profisafe/6_1_condition.png)
4) 验证 **TIA Portal** 中和 **General I/O** 屏幕上的 I/O 信号。<br>
![](../../../_assets/safetyio_profisafe/6_3_public_io.png)

#### 4.7) PROFIsafe I/O 信号的分配
1) PROFIsafe I/O 信号的分配
* 请参阅 **[3.3.4.3 Safety Signal Assignment](../4-safety-io/3-Linker.md)** 页面。

2) PROFIsafe I/O 信号分配示例
<br>
<br>2-1) PROFIsafe 输入（方向：主 -> 从）
<br><br>
[将 0 位设置为臂限制] <br>
![](../../../_assets/safetyio_profisafe/7_PS_in.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/7_PS_in2.png)
<br> <br>
2-2) PROFIsafe 输出（方向：从 -> 主）
<br> <br>
[将 0 位设置为紧急停止状态]<br>
![](../../../_assets/safetyio_profisafe/7_PS_out.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/7_PS_out2.png)