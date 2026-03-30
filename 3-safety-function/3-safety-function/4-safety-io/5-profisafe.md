# 3.3.4.5 PROFIsafe

## 1) PROFIsafe?
- 一种在PROFINET/PROFIBUS上运行的安全协议（安全配置文件）。
- 通过标准PROFINET通信通道（“黑色通道”）传输安全数据。
- 支持安全信号传输，无需额外布线。

## 2) PROFINET & PROFIsafe 规格
- 数字输入：50、120或240字节（选择一个）
- 数字输出：50、120或240字节（选择一个）
- 安全I/O：8/8字节（启用或禁用）
- 最小通信周期：1毫秒
- 支持的通信速度：10或100 Mbps
- 兼容性类别：B
- 净负载类别：II
- 可选功能：遗留，MRP

## 3) PROFIsafe 参数

`[System > 2: Control Parameters > 11: Industrial Communication > 6: Safety Communication > 2: PROFIsafe]`<br>
![](../../../_assets/safetyio_profisafe/profisafe_param.png)

 - 源地址：设置源地址。（固定为1）
 - 目标地址：设置目标地址。（设置范围：1到65534）

 ***注意***<br> 
 - 地址类型：地址类型1（仅允许目标地址）
 - 设备故障反应：如果该设备进入故障状态，所有F-输出将变为安全故障（0）状态。一旦设备的故障状态被解决，需要通过F-主机发出的Global-Acknowledge等命令进行F-设备的重新整合。

## 4) PROFIsafe 配置程序

1) BD671与F-Host & Hi7 Com之间的连接
2) GSDML 文件注册（TIA Portal）
3) PROFIsafe 控制器配置（TIA Portal）
<br>3.1) PROFINET 配置
<br>3.2) PROFIsafe 配置
4) Hi7 配置（TP UI）
<br>4.1) PROFINET 配置
<br>4.2) PROFIsafe 配置
5) 验证 PROFINET 和 PROFIsafe 通信
6) PROFINET I/O信号的分配（FB块设置）
7) PROFIsafe I/O信号的分配

### 4.1) BD671 和 F-Host & Hi7 Com 之间的连接

#### 4.1.1) LAN 电缆连接
1) 使用LAN电缆将“PROFIsafe F-Host”和BD671连接。
2) 验证链路LED是否闪烁。
3) 使用LAN电缆将Hi7 COM的LAN3连接器与BD671连接。
4) 验证链路LED是否闪烁。

![](../../../_assets/safetyio_profisafe/profisafe_connect.png)

#### 4.1.2) Hi7 Com 连接设置
1) 导航到以下菜单：**System -> Control Parameters -> Industrial Communication -> EtherCAT Master Settings**
2) 您的设置如下：
- EtherCAT主站：开启
- 端口：LAN3
3) 从从站列表中选择“OptionBD - PROFINET_IO”，并按**应用**按钮。
4) 重启Hi7机器人控制器。
5) 重启后检查**运行**、**通信**和**错误**LED的状态。

![](../../../_assets/safetyio_profisafe/EC_master_setting1.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/EC_master_setting2.png)

### 4.2) GSDML 文件注册（TIA Portal）
1) 启动TIA Portal。
2) 导航到右侧菜单：**[Options] → [Manage general station description file (GSD)]**。
3) 点击**"..."**按钮，选择GSDML文件所在目录。
4) 从显示的列表中选择**"GSDML-V2.43-Hyundai-Robotics-HI6-20251127.xml"**并点击**[安装]**按钮。
5) 验证该文件已在硬件目录中注册为新设备。 <br>
![](../../../_assets/safetyio_profisafe/profisafe_gsdmal.png)

### 4.3) PROFIsafe 控制器配置（TIA Portal）
#### 4.3.1) PROFINET 配置
1) 启动TIA Portal并创建新项目。
2) 双击**Devices & Networks**以打开它。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network.png)

3) 选择支持PROFINET通信的控制器（例如，CPU 1511F-1 PN），并将其拖入**网络视图**。
4) 从硬件目录中选择上一步添加的设备（HRC，PROFINET I/O DAP）并将其拖入**网络视图**。
5) 在图中通过拖放连接两个设备的相应LAN端口。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network2.png)

6) 双击**"Devices & Networks"**视图中的HRC-IO设备。
7) 选择所需的插槽。
8) 从右侧目录中拖动所需模块（DI、DO或PROFIsafe I/O）并移动到**"Device Overview"**窗口。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network3.png)

9) 双击**"Devices & Networks"**视图中的HRC-IO设备。
10) 再次单击HRC-IO设备以打开**属性**（设置）窗口。
11) 导航到底部的**常规**标签。
12) 从左侧菜单中选择**以太网地址**。
13) 取消选中**"自动生成PROFINET设备名称"**选项。
14) 将**"PROFINET设备名称"**设置为**"hd-hrc-hi7"**并保存更改。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network4.png)

#### 4.3.2) PROFIsafe 配置
1) 双击**"Devices & Networks"**视图中的HRC-IO设备。
2) 在右侧的**"Device Overview"**窗口中选择PROFIsafe插槽。
3) PROFIsafe通信设置将在下方窗格中显示。
4) 点击**PROFIsafe**标签。
5) 将**F_Dest_Add**设置为1。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network5.png)

### 4.4) Hi7 配置（TP UI）
#### 4.4.1) PROFINET 配置
1) 使用与F-Host中设置相同的值配置参数：
- PROFINET IO设备名称：hd-hrc-hi7
- 插槽1：数字输入：240
- 插槽2：数字输出：240
- 插槽3：安全I/O：已选择
2) 按**"应用"**按钮。<br>
![](../../../_assets/safetyio_profisafe/4_1_profinet_config.png)

#### 4.4.2) PROFIsafe 配置

1) 将**目标地址**设置为1，使用前面部分配置的相同值。
2) 按**"应用"**按钮。<br>
![](../../../_assets/safetyio_profisafe/4_2_profisafe_config.png)

### 4.5) 验证 PROFINET 和 PROFIsafe 通信

### 4.5.1) 安全梯形程序（TIA Portal）
1) 在**设备概览**选项卡中，创建如下所示的梯形程序并下载到控制器中。<br>
![](../../../_assets/safetyio_profisafe/5_1_Safety_Ladder.png)
2) 下载后，验证**分布式 I/O**屏幕上是否显示绿色复选框。<br>
![](../../../_assets/safetyio_profisafe/5_1_Safety_Ladder2.png)

### 4.5.2) TP 屏幕
1) PROFINET <br>
导航到**System -> 2: Control Parameters -> 11: Industrial Communication -> 5: PROFINET Settings**菜单中。<br>
![](../../../_assets/safetyio_profisafe/5_2_pnio_status.png)
- 检查每个插槽的状态信息。
- 验证计数器是否持续增加。

2) PROFIsafe <br>
导航到**System > 2: Control Parameters > 11: Industrial Communication > 6: Safety Communication > 2: PROFIsafe**菜单中。<br>
![](../../../_assets/safetyio_profisafe/5_2_profisafe_status.png)
- 验证**FappState**是否设置为**CYCLE Data EX**。
- 验证**计数器**是否持续增加。

### 4.6) PROFINET I/O 信号的分配（FB 块设置）
1) 导航到**System → Control Parameters → I/O Signal Settings → FB Block Assignment**。
2) 根据需要将块设置更改为**PROFINET I/O**，最多可设置2个块。
 （最大PROFINET I/O大小为240字节，每个单独FB块的大小为120字节。因此，**超过2个块的任何设置将被忽略。**）<br>
![](../../../_assets/safetyio_profisafe/6_fb_block.png)

3) 另外，导航到**条件设置**菜单并验证**PLC操作模式**设置为**OFF**。<br>
![](../../../_assets/safetyio_profisafe/6_1_condition.png)
4) 验证**TIA Portal**中的I/O信号和**General I/O**屏幕中的信号。<br>
![](../../../_assets/safetyio_profisafe/6_3_public_io.png)

### 4.7) PROFIsafe I/O信号的分配
1) PROFIsafe I/O信号的分配
* 请参考**[3.3.4.3 Safety Signal Assignment](../4-safety-io/3-Linker.md)**页面。

2) PROFIsafe I/O信号分配的示例
<br>
<br>2-1) PROFIsafe输入（方向：主设备 -> 从设备）
<br><br>
[将0位设置为臂限制] <br>
![](../../../_assets/safetyio_profisafe/7_PS_in.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/7_PS_in2.png)
<br> <br>
2-2) PROFIsafe输出（方向：从设备 -> 主设备）
<br> <br>
[将0位设置为紧急停止状态]<br>
![](../../../_assets/safetyio_profisafe/7_PS_out.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/7_PS_out2.png)