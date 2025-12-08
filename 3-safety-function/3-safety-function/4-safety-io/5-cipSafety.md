

# 3.3.4.5 CIP Safety

## 1. CIP Safety ?
- CIP Safety是在标准Common Industrial Protocol（CIP）基础上扩展而成的安全通信协议。
- 使用“黑通道”原理，可在EtherNet/IP和DeviceNet上进行安全数据交换。
- 通过时间监控、冗余、CRC检查等机制，符合IEC 61508、ISO 13849等安全标准。

## 2. 规格
### 2.1 EtherNet/IP
- 数字输入 : 0 ~ 240 bytes
- 数字输出 : 0 ~ 240 bytes
- 通信周期 : 1 ~ 3000 msec
- 支持通信速度 : 10或100 Mbps

### 2.2 CIP Safety
- 安全输入输出 : 8/8 bytes 
- 通信周期 : 20 ~ 100 msec


## 3. CIP Safety参数

![](../../../_assets/cipSafety/cipSafety_Parameters.png)

 - 使用/未使用:决定是否使用CIP Safety功能。
 - SNN:设置Safety Network Number。
 - Configure Signature : Reserved



## 4. CIP Safety设置流程

1) Hi7 EtherNet/IP Adapter与EtherNet/IP Scanner的连接
2) 通过工程工具添加EDS文件（Studio 5000）
3) CIP Safety控制器设置（Studio 5000）
4) Hi7设置（TP UI）
4.1) EtherNet/IP设置
4.2) CIP Safety设置
5) EtherNet/IP与CIP Safety通信状态的确认
6) 安全信号的分配


### 1 Hi7 EtherNet/IP Adapter与EtherNet/IP Scanner的连接
![](../../../_assets/cipSafety/connect.png)

### 2 通过工程工具添加EDS文件（Studio 5000）
- 使用“Device Description File Installation Tool”安装EDS（Hi7_EIP_250203.eds）文件。
### 3 CIP Safety控制器设置（Studio 5000）
1) 执行Studio 5000并创建新项目。
2) 在controller organizer中选择支持CIP Safety通信的控制器（如CPU 1769-L30ERMS)，并选择Ethernet后右击New Module。
3) 找到“Hi7 EIP Adapter”并点击“Create”按钮。<br>
![CIP Safety](../../../_assets/cipSafety/new_module.png)

4) 在Name栏中设置设备名称。
5) IP Address设置为：例）192.168.4.150。
6) Safety Network Number设置为：例）1111_2222_3333。<br>
![CIP Safety](../../../_assets/cipSafety/Setting_SNN.png)


7) 在Module Definition中点击“Change”按钮后，设置Safety I/O及标准I/O大小。
- Standard I/O（Exclusive owner）：240 bytes
- Safety I/O : 各8 bytes
8) 请勿设置“Configuration signature”。
9) 请关闭Select Module type窗口。<br>
![CIP Safety](../../../_assets/cipSafety/Setting_module.png)
10) 请确认模块已添加。<br>
![CIP Safety](../../../_assets/cipSafety/module_added.png)
11) 在工具栏菜单中，请点击“offline”按钮后，再点击“Download”按钮。<br>
![CIP Safety](../../../_assets/cipSafety/download.png)
12) 在设定值下载完成后，请将“Guard Logix”的拨动开关从PROG切换到RUN。
### 4 Hi7设置（TP UI）
#### 4.1 EtherNet/IP设置
1) 依次进入菜单：系统 → 控制参数 → 工业通信 → EtherNet/IP设置
2) Protocol设置 = Adapter
3) 用于EtherNet/IP Adapter的LAN端口设置为LAN2。
4) Input/Output大小各设置为240字节。
5) 其余设置不做更改，如图所示。<br>
![CIP Safety](../../../_assets/cipSafety/ethernetIP.png)

#### 4.2 CIP Safety设置
1) 依次进入菜单：系统 → 安全系统 → 参数设置 → 安全输入输出 → CIP Safety。
2) 启用按钮ON
3) SNN设置为：例)1111_2222_3333。
4) 点击“应用”按钮。
5) 重启机器人控制器。<br>
![CIP Safety](../../../_assets/cipSafety/cipSafety_Parameters.png)
### 5. 通信状态确认
#### 5.1 EtherNet/IP
1) 确认License Led点亮
2) 确认Run Led点亮
3) 确认Communication Led点亮
4) 当Error Led点亮时则确认Error Name<br>
![CIP Safety](../../../_assets/cipSafety/eip_status.png)
#### 5.2 CIP Safety
1) 确认Dev status是否为“Executing”状态
2) 确认Comm status是否为“On-line, Connected”状态
3) 确认IO Count是否持续递增<br>
![CIP Safety](../../../_assets/cipSafety/cipsafety_status.png)

### 6 安全信号的分配
#### 6.1 CIP Safety输入输出的分配<br>
* 参考 [3.3.3.3 安全信号分配](3-safety-function/3-safety-function/3-safety-io/3-Linker.md) 页面
#### 6.2 CIP Safety输入输出分配示例
1) CIP Safety Input（Master -> Slave方向）
1ch(0 bit) = Arm Limit<br>
![CIP Safety](../../../_assets/cipSafety/alloc_in.png)<br>
<br> <br>
![CIP Safety](../../../_assets/cipSafety/alloc_in2.png)<br>

2) CIP Safety Output（Slave -> Master方向）
1ch(0 bit) = E-Stop Status<br>
![CIP Safety](../../../_assets/cipSafety/alloc_out.png)<br>
<br> <br>
![CIP Safety](../../../_assets/cipSafety/alloc_out2.png)<br>

