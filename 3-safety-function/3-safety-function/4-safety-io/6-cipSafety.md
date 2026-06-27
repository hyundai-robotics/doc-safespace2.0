# 3.3.4.6 CIP Safety

### 1) 什么是 CIP Safety?
- **CIP Safety** 是一种安全通信协议，扩展了标准的 **Common Industrial Protocol (CIP)**。
- 它通过利用 **"Black Channel"** 原则，支持在 **EtherNet/IP** 和 **DeviceNet** 上进行安全数据交换。
- 它通过时间监控、冗余和 CRC（循环冗余检查）等机制，符合 **IEC 61508** 和 **ISO 13849** 等国际安全标准。
<br>
<br>

### 2) 规格
#### 2.1) EtherNet/IP
- **数字输入：** 0 ~ 240 字节
- **数字输出：** 0 ~ 240 字节
- **RPI（请求包间隔）：** 5 ~ 3000 毫秒
- **支持的通信速度：** 10 或 100 Mbps

#### 2.2) CIP Safety
- **安全 I/O：** 8/8 字节
- **RPI（请求包间隔）：** 20 ~ 100 毫秒
<br>
<br>

### 3) CIP Safety 参数
`[System > 2: Control Parameters > 11: Industrial Communication > 6: Safety Communication > 3: CIP Safety]`<br>
![](../../../_assets/cipSafety/cipSafety_Parameters.png)

 - **安全网络编号：** 设置安全网络编号 (SNN)。
 - **IP 地址：** 显示当前配置的 EtherNet/IP 适配器的 IP 地址。
 <br>{% hint style="info" %}
* 如果 EtherNet/IP 适配器的 IP 地址被更改，必须执行 **"Apply All"** 以更新 CIP Safety 参数。
{% endhint %}
 
   

### 4) CIP Safety 配置过程

1) 建立 Hi7 EtherNet/IP 适配器与 EtherNet/IP 扫描器之间的连接。
2) 通过工程工具（Studio 5000）添加 EDS 文件。
3) 配置 CIP Safety 控制器（Studio 5000）。
4) 配置 Hi7（TP UI）。
   4.1) EtherNet/IP 配置
   4.2) CIP Safety 配置
5) 验证 EtherNet/IP 和 CIP Safety 通信状态。
6) 分配安全信号。


#### 4.1) Hi7 EtherNet/IP 适配器与 EtherNet/IP 扫描器之间的连接
![](../../../_assets/cipSafety/connect.png)

#### 4.2) 通过工程工具（Studio 5000）添加 EDS 文件
- 使用 **'Device Description File Installation Tool'** 安装 EDS 文件 (**Hi7_EIP_251023.eds**)。

#### 4.3) CIP Safety 控制器配置（Studio 5000）
1) 启动 **Studio 5000** 并创建新项目。
2) 在 **Controller Organizer** 中，选择支持 CIP Safety 通信的控制器（例如，CPU 1769-L30ERMS）。右键单击 **Ethernet** 并点击 **New Module**。
3) 搜索 **"Hi7 EIP Adapter"** 并点击 **Create** 按钮。<br>
![CIP Safety](../../../_assets/cipSafety/new_module.png)

4) 在 **Name** 字段中输入设备名称。
5) 设置 **IP 地址**（例如，192.168.4.150）。
6) 设置 **安全网络编号**（例如，1111_2222_3333）。<br>
![CIP Safety](../../../_assets/cipSafety/Setting_SNN.png)


7) 点击 **Module Definition** 中的 **Change** 按钮以配置安全 I/O 和标准 I/O 的大小。
- **标准 I/O（独占所有者）：** 240 字节
- **安全 I/O：** 每个 8 字节
8) 不要配置 **"Configuration signature"**。
9) 关闭 **Select Module Type** 窗口。<br>
![CIP Safety](../../../_assets/cipSafety/Setting_module.png)

10) 验证模块是否成功添加。<br>
![CIP Safety](../../../_assets/cipSafety/module_added.png)

11) 在工具栏菜单中点击 **Offline** 按钮，然后点击 **Download**。<br>
![CIP Safety](../../../_assets/cipSafety/download.png)

12) 在配置值下载后，将 **GuardLogix** 切换开关从 **PROG** 切换到 **RUN** 模式。

#### 4.4) Hi7 配置（TP UI）
##### 4.4.1) EtherNet/IP 配置
1) 导航至 **System → Control Parameters → Industrial Communication → EtherNet/IP Settings**。
2) 将 **Protocol** 设置为 **Adapter**。
3) 将 EtherNet/IP 适配器的 LAN 端口设置为 **LAN2**。
4) 将 **Input** 和 **Output** 大小均设置为 **240 字节**。
5) 不要更改其余设置，保持如图所示。<br>
![CIP Safety](../../../_assets/cipSafety/ethernetIP.png)

##### 4.4.2) CIP Safety 配置
1) 导航至 **System → 2: Control Parameters → 11: Industrial Communication → 6: Safety Communication → 3: CIP Safety**。
2) 将 **Activation** 按钮设置为 **ON**。
3) 将 **SNN**（例如，1111_2222_3333）设置为与 Studio 5000 中配置的值匹配。
4) 点击 **Apply** 按钮。
5) **重启** 机器人控制器。<br>
![CIP Safety](../../../_assets/cipSafety/cipSafety_Parameters.png)

#### 4.5) 验证通信状态
##### 4.5.1) EtherNet/IP
1) 验证 **License LED** 是否亮起。
2) 验证 **Run LED** 是否亮起。
3) 验证 **Communication LED** 是否亮起。
4) 如果 **Error LED** 亮起，请检查 **Error Name** 获取详细信息。<br>
![CIP Safety](../../../_assets/cipSafety/eip_status.png)

##### 4.5.2) CIP Safety
1) 验证 **Safety Communication** 是否设置为 **"CIP Safety"**。
2) 验证 **Comm status** 是否处于 **"On-line, Connected"** 状态。
3) 验证 **IO Count** 是否持续增加。<br>
![CIP Safety](../../../_assets/cipSafety/cipsafety_status.png)

#### 4.6) 安全信号分配
##### 4.6.1) CIP Safety I/O 的分配<br>
* 请参考 **[3.3.4.3 Safety Signal Assignment](../4-safety-io/3-Linker.md)** 页面。

##### 4.6.2) CIP Safety I/O 分配示例
1) CIP Safety 输入（方向：主站 -> 从站）
1ch(0 bit) = 臂限制<br>
![CIP Safety](../../../_assets/cipSafety/alloc_in.png)<br>
<br> <br>
![CIP Safety](../../../_assets/cipSafety/alloc_in2.png)<br>

2) CIP Safety 输出（方向：从站 -> 主站）
1ch(0 bit) = 紧急停止状态<br>
![CIP Safety](../../../_assets/cipSafety/alloc_out.png)<br>
<br> <br>
![CIP Safety](../../../_assets/cipSafety/alloc_out2.png)<br>