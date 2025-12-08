

# 3.3.4.4 PROFIsafe

## 1. PROFIsafe ?
- 在PROFINET/PROFIBUS上运行的安全协议（安全配置文件）。
- 通过标准PROFINET通信通道（“黑通道”）传输安全数据。
- 支持无需额外布线的安全信号传输。

## 2. PROFINET & PROFIsafe规格
- 数字输入：50、120、240 bytes（选择1个）
- 数字输出：50、120、240 bytes（选择1个）
- 安全输入输出：8/8 bytes（启用或禁用）
- 最小通信周期：1 msec
- 支持通信速度：10或100 Mbps
- Conformance Class : B
- Netload Class : II
- Optional Feature : Legacy, MRP

## 3. PROFIsafe参数

![](../../../_assets/safetyio_profisafe/profisafe_param.png)

 - Source Address：设置Source Address。（固定为1）
 - Target Address：设置Target Address。（设置范围：1 ~ 99）

  ***参考事项*** 
 - Address Type :  Address Type 1（仅检查Destination Address）
 - Reaction on Device_Fault：当该装置处于Fault状态时，所有F-Output输出都会变更为Fail-safe（0）状态。而且，该装置的Fault状态解除后，需要在F-Host使用Global-Acknowledge等指令对F-Device进行re-integration的过程。


## 4. PROFIsafe设置流程

1) BD671与F-Host & Hi7 Com的连接
2) GSDML文件注册（TIA Portal）
3) PROFIsafe控制器设置（TIA Portal）
<br>3.1) PROFINET设置
<br>3.2) PROFIsafe设置
4) Hi7设置（TP UI）
<br>4.1) PROFINET设置
<br>4.2) PROFIsafe设置
5) PROFINET与PROFIsafe通信的确认
6) PROFINET I/O信号分配(FB Block Settings)
7) PROFIsafe I/O信号的分配


### 4.1 BD671与F-Host & Hi7 Com的连接

#### 4.1.1 网线连接
1) 用网线连接“PROFIsafe F-Host”与BD671。
2) 确认Link LED是否闪烁。
3) 用网线连接Hi7 COM的LAN3连接器与BD671。
4) 确认Link LED是否闪烁。

![](../../../_assets/safetyio_profisafe/profisafe_connect.png)

#### 4.1.2 Hi7 Com的连接设置
1) 依次进入菜单：系统 -> 控制参数 -> 工业通信-> EtherCAT Master设置
2) 按如下所示进行设置：
- EtherCAT Master : ON
- Port : LAN3
3) 在从站列表中选择“OptionBD – PROFINET_IO”并按下应用按钮。
4) 重启Hi7机器人控制器。
5) 重启后确认Run & Communication & Error LED的点亮状态。

![](../../../_assets/safetyio_profisafe/EC_master_setting1.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/EC_master_setting2.png)


### 4.2 GSDML文件注册（TIA Portal）
1) 执行TIA Portal
2) 如右侧所示，依次进入菜单：[Options] → [Manage general station description file (GSD)].
3) 点击“…”按钮后，设置GSDML file所在的目录。
4) 从屏幕显示的列表中，选择“GSDML-V2.43-Hyundai-Robotics-HI6-20250418.xml”并按下[Install]按钮。
5) 确认其是否在硬件目录中注册为新设备。 <br>
![](../../../_assets/safetyio_profisafe/profisafe_gsdmal.png)

### 4.3 PROFIsafe控制器设置（TIA Portal）
#### 4.3.1 PROFINET设置
1) 执行TIA Portal并创建新项目。
2) 双击Device & Network部分来将其打开。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network.png)

3) 选择支持PROFIsafe通信的控制器（例如CPU 1511F-1 PN）并拖放到网络视图。
4) 从硬件目录中添加上一步骤添加的设备（HRC、PROFINET I/O DAP）并拖放到网络视图。
5) 通过鼠标拖放将两个设备图中的LAN端口相互连接。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network2.png)

6) 在“Device & Network”界面中双击HRC-IO设备。
7) 选择所需的插槽。
8) 从右侧目录中将所需的模块（DI、 DO或PROFIsafe I/O）拖动到“Device Overview window”。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network3.png)

9) 在“Device & Network”界面中双击HRC-IO设备。
10) 再次点击HRC-IO设备来打开Setting界面。
11) 移动到下面的General标签。
12) 在左侧菜单中选择Ethernet addresses。
13) 取消勾选“Generate PROFINET device name automatically.”部分。
14) 将“PROFINET device name”设置为“hd-hrc-0”并保存。<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network4.png)

#### 4.3.2 PROFIsafe设置
1） 在“Device & Network”界面中双击HRC-IO设备。
2) 在右侧“Device Overview”屏幕中选择PROFIsafe插槽。
3) 下方屏幕中显示PROFIsafe通信设置界面。
4) 点击PROFIsafe选项卡
5) 将F_Dest_Add设置为1


### 4.4 Hi7设置（TP UI）
#### 4.4.1 PROFINET设置
1) 使用与F-Host中设置的相同值（如下数值）来设置参数
- PROFINET IO Device Name : hd-hrc-0
- Slot 1 : Digital Input : 240
- Slot 2 : Digital Output : 240
- Slot 3 : Safety I/O : Yes
- （IP地址无需更改。）
2) 按“应用”按钮。<br>
![](../../../_assets/safetyio_profisafe/4_1_profinet_config.png)

#### 4.4.2 PROFIsafe设置

1) 使用与上一章节中设置的相同值，将Target Address设置为1。
2) 按“应用”按钮。<br>
![](../../../_assets/safetyio_profisafe/4_2_profisafe_config.png)

### 4.5 PROFINET与PROFIsafe通信的确认

### 4.5.1 安全梯形图程序（Tia Portal）
1) 在Device Overview选项卡中，创建如下梯形图程序并下载到控制器。<br>
![](../../../_assets/safetyio_profisafe/5_1_Safety_Ladder.png)
2) 下载后，在Distribution I/O界面中确认是否显示绿色复选框。<br>
![](../../../_assets/safetyio_profisafe/5_1_Safety_Ladder2.png)

### 4.5.2 TP界面
1) PROFINET
从菜单中移动到：系统 -> 安全系统 -> 监控 -> PROFINET状态。<br>
![](../../../_assets/safetyio_profisafe/5_2_pnio_status.png)
- 确认各插槽的状态信息。
- 确认Counter是否持续递增。

2) PROFIsafe
在菜单中进入：系统 -> 安全系统 -> 监视 -> PROFIsafe状态。<br>
![](../../../_assets/safetyio_profisafe/5_2_profisafe_status.png)
- 确认FappState是否为CYCLE Data EX
- 确认Counter是否持续递增。

### 4.6 PROFINET I/O信号分配（FB Block Settings）
1) 依次进入：系统 → 控制参数 → 输入输出信号设置 → FB块分配
2) 将所需数量的块设置更改为PROFINET I/O，数量不得超过2个。
 （最大PROFINET I/O大小为240字节，单个FB块的大小为120字节。因此，**超过2个的设置将被忽略。**）<br>
![](../../../_assets/safetyio_profisafe/6_fb_block.png)

3) 另外，移动到条件设置菜单并确认PLC运行模式是否为OFF。<br>
![](../../../_assets/safetyio_profisafe/6_1_condition.png)
4) 在TIA Portal及通用I/O界面中，确认输入输出信号。<br>
![](../../../_assets/safetyio_profisafe/6_3_public_io.png)

### 4.7 PROFIsafe I/O信号的分配
1) PROFIsafe I/O信号的分配
* 参考 [3.3.4.3 安全信号分配](../4-safety-io/3-Linker.md) 页面

2) PROFIsafe I/O信号分配示例
<br>
<br>2-1) PROFIsafe输入（Master -> Slave方向）
[将1ch（0 bit）设置为Arm Limit] <br>
![](../../../_assets/safetyio_profisafe/7_PS_in.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/7_PS_in2.png)
<br> <br>
2-2) PROFIsafe输出（Slave -> Master方向）
<br> <br>
[将1ch（0 bit）设置为紧急停止状态]<br>
![](../../../_assets/safetyio_profisafe/7_PS_out.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/7_PS_out2.png)



