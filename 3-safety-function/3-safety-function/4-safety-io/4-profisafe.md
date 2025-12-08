

# 3.3.4.4 PROFIsafe

## 1. PROFIsafe ?
- A safety protocol (safety profile) that operates on PROFINET/PROFIBUS.
- Transmits safety data through the standard PROFINET communication channel ('Black Channel').
- Supports safety signal transmission without additional wiring.

## 2. PROFINET & PROFIsafe Specifications
- Digital input: 50, 120, and 240 bytes (select one type of byte count)
- Digital output: 50, 120, and 240 bytes (select one type of byte count)
- Safety I/O: 8/8 bytes (activated or deactivated)
- Minimum communication cycle: 1 msec
- Supported communication speed: 10 or 100 Mbps
- Conformance Class : B
- Netload Class : II
- Optional Feature : Legacy, MRP

## 3. PROFIsafe Parameters

![](../../../_assets/safetyio_profisafe/profisafe_param.png)

 - Source Address: Sets the Source Address. (Fixed to 1.)
 - Target Address: Sets the Target Address (Setting range: 1–99).

  ***Notes*** 
 - Address Type :  Address Type 1 (Checks Destination Address only)
 - Reaction on Device_Fault : When this device enters Fault state, all F-Output outputs change to Fail-safe (0) state. After the device's Fault state is resolved, a process such as Global-Acknowledge from the F-Host is required to re-integrate the F-Device.


## 4. PROFIsafe Configuration Procedure

1) Connection of BD671, F-Host and Hi7 Com
2) GSDML file registration (TIA portal)
3) PROFIsafe Controller Settings (TIA Portal)
<br>3.1) PROFINET Settings
<br>3.2) PROFIsafe Settings
4) Hi7 settings (TP UI)
<br>4.1) PROFINET Settings
<br>4.2) PROFIsafe Settings
5) Verification of PROFINET and PROFIsafe Communication
6) PROFINET I/O signal assignment (FB block settings)
7) PROFIsafe I/O Signal Assignment


### 4.1 Connection of BD671, F-Host and Hi7 Com

#### 4.1.1 LAN Cable Connection
1) Connect the "PROFIsafe F-Host" to BD671 with a LAN cable.
2) Check if the Link LED is blinking.
3) Connect the Hi7 COM’s LAN3 connector and BD671 using a LAN cable.
4) Check if the Link LED is blinking.

![](../../../_assets/safetyio_profisafe/profisafe_connect.png)

#### 4.1.2 Hi7 Com Connection Settings
1) Navigate to the menu as follows: System -> Control Parameters -> Industrial Communication -> EtherCAT Master Settings
2) Configure as shown below.
- EtherCAT Master : ON
- Port : LAN3
3) Select "OptionBD – PROFINET_IO" from the slave list and press the Apply button.
4) Reboot the Hi7 robot controller.
5) After rebooting, check the status of the Run, Communication, Error LEDs.

![](../../../_assets/safetyio_profisafe/EC_master_setting1.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/EC_master_setting2.png)


### 4.2 GSDML File Registration (TIA portal)
1) Run the TIA portal.
2) Navigate as shown on the right in the menu: [Options] → [Manage general station description file (GSD)].
3) Click the "…" button and set the directory where the GSDML file is located.
4) Select "GSDML-V2.43-Hyundai-Robotics-HI6-20250418.xml" from the list displayed on the screen and press the [Install] button.
5) Check if it has been registered as a new device in the hardware catalog. <br>
![](../../../_assets/safetyio_profisafe/profisafe_gsdmal.png)

### 4.3 PROFIsafe Controller Settings (TIA Portal)
#### 4.3.1 PROFINET Settings
1) Run the TIA portal and create a new project.
2) Double-click the Device & Network section to open it.<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network.png)

3) Select a controller that supports PROFIsafe communication (e.g. CPU 1511F-1 PN) and drag it to the network view.
4) Add the device (HRC, PROFINET I/O DAP) added in the previous step from the hardware catalog and drag it to the network view.
5) Connect the two devices by dragging and dropping the LAN ports in the two device figures.<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network2.png)

6) Double-click the HRC-IO device in the "Device & Network" screen.
7) Select the desired slot.
8) Drag the desired module (DI, DO, or PROFIsafe I/O) from the catalog on the right and move it to the "Device Overview window."<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network3.png)

9) Double-click the HRC-IO device in the "Device & Network" screen.
10) Click the HRC-IO device again to open the Settings screen.
11) Navigate to the General tab below.
12) Select Ethernet addresses from the menu on the left.
13) Uncheck "Generate PROFINET device name automatically."
14) Set "PROFINET device name" to "hd-hrc-0" and save.<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network4.png)

#### 4.3.2 PROFIsafe Settings
1) Double-click the HRC-IO device in the "Device & Network" screen.
2) Select the PROFIsafe slot in the "Device Overview" screen on the right.
3) The PROFIsafe communication settings screen appears on the bottom screen.
4) Click the PROFIsafe tab.
5) Set F_Dest_Add to 1.


### 4.4 Hi7 Settings (TP UI)
#### 4.4.1 PROFINET Settings
1) Set the parameters with the same values as set in the F-Host as follows:
- PROFINET IO Device Name : hd-hrc-0
- Slot 1 : Digital Input : 240
- Slot 2 : Digital Output : 240
- Slot 3 : Safety I/O : Yes
- (No need to change the IP address.)
2) Press the "Apply" button.<br>
![](../../../_assets/safetyio_profisafe/4_1_profinet_config.png)

#### 4.4.2 PROFIsafe Settings

1) Set the Target Address to 1 with the same value as set in the previous chapter.
2) Press the "Apply" button.<br>
![](../../../_assets/safetyio_profisafe/4_2_profisafe_config.png)

### 4.5 Verification of PROFINET and PROFIsafe Communication

### 4.5.1 Safety Ladder Program (Tia Portal)
1) In the Device Overview tab, create a ladder program as shown below and download it to the controller.<br>
![](../../../_assets/safetyio_profisafe/5_1_Safety_Ladder.png)
2) After downloading, check if a green checkbox is displayed on the Distribution I/O screen.<br>
![](../../../_assets/safetyio_profisafe/5_1_Safety_Ladder2.png)

### 4.5.2 TP Screen
1) PROFINET
In the menu, navigate to System -> Safety System -> Monitoring -> PROFINET Status.<br>
![](../../../_assets/safetyio_profisafe/5_2_pnio_status.png)
- Check the status information of each slot.
- Check if the counter continuously increases.

2) PROFIsafe
In the menu, navigate to System -> Safety System -> Monitoring -> PROFIsafe Status.<br>
![](../../../_assets/safetyio_profisafe/5_2_profisafe_status.png)
- Check if FappState is CYCLE Data EX.
- Check if the counter continuously increases.

### 4.6 PROFINET I/O Signal Assignment (FB block settings)
1) Navigate to System → Control Parameters → Input/Output Signal Settings → FB Block Assignment
2) Change the block settings to PROFINET I/O as many as needed (up to two).
 (The maximum PROFINET I/O size is 240 bytes and the individual FB block size is 120 bytes. Therefore, **any settings exceeding two will be ignored.**)<br>
![](../../../_assets/safetyio_profisafe/6_fb_block.png)

3) Additionally, navigate to the Condition Settings menu and check if the PLC operation mode is OFF.<br>
![](../../../_assets/safetyio_profisafe/6_1_condition.png)
4) Check the input/output signals on the TIA portal screen and General I/O screen.<br>
![](../../../_assets/safetyio_profisafe/6_3_public_io.png)

### 4.7 PROFIsafe I/O Signal Assignment
1) PROFIsafe I/O Signal Assignment
* Refer to [3.3.4.3 Safety Signal Assignment](../4-safety-io/3-Linker.md) page

2) PROFIsafe I/O Signal Assignment Example
<br>
<br>2-1) PROFIsafe Input (Direction: Master -> Slave)
[Set 1ch(0 bit) to Arm Limit] <br>
![](../../../_assets/safetyio_profisafe/7_PS_in.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/7_PS_in2.png)
<br> <br>
2-2) PROFIsafe Output (Direction: Slave -> Master)
<br> <br>
[Set 1ch(0 bit) to Emergency Stop Status]<br>
![](../../../_assets/safetyio_profisafe/7_PS_out.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/7_PS_out2.png)



