

# 3.3.4.5 CIP Safety

## 1. CIP Safety ?
- CIP Safety is a safety communication protocol that extends the standard Common Industrial Protocol (CIP).
- Enables safe data exchange on EtherNet/IP and DeviceNet using the 'Black Channel' principle.
- Complies with safety standards such as IEC 61508 and ISO 13849 through mechanisms like time monitoring, redundancy, and CRC checks.

## 2. Specifications
### 2.1 EtherNet/IP
- Digital Input: 0–240 bytes
- Digital Output: 0–240 bytes
- Communication Cycle: 1–3000 msec
- Supported communication speed: 10 or 100 Mbps

### 2.2 CIP Safety
- Safety I/O: 8/8 bytes
- Communication Cycle: 20–100 msec


## 3. CIP Safety Parameters

![](../../../_assets/cipSafety/cipSafety_Parameters.png)

 - Enable/Disable: Determines whether to use the CIP Safety function.
 - SNN: Sets the Safety Network Number.
 - Configure Signature : Reserved



## 4. CIP Safety Setting Procedure

1) Connection of Hi7 EtherNet/IP Adapter and EtherNet/IP Scanner
2) Addition of an EDS file through the engineering tool (Studio 5000)
3) CIP Safety Controller Settings (Studio 5000)
4) Hi7 settings (TP UI)
4.1) EtherNet/IP Settings
4.2) CIP Safety Settings
5) Checking of EtherNet/IP and CIP Safety Communication Status
6) Assignment of Safety Signal


### 1 Connection of Hi7 EtherNet/IP Adapter and EtherNet/IP Scanner
![](../../../_assets/cipSafety/connect.png)

### 2 Addition of an EDS file through the engineering tool (Studio 5000)
- Install the EDS (Hi7_EIP_250203.eds) file using the 'Device Description File Installation Tool.'
### 3 CIP Safety Controller Settings (Studio 5000)
1) Run Studio 5000 and create a new project.
2) In the controller organizer, select a controller that supports CIP Safety communication (e.g. CPU 1769-L30ERMS), select Ethernet, right-click and click New Module.
3) Find "Hi7 EIP Adapter" and press the Create button.<br>
![CIP Safety](../../../_assets/cipSafety/new_module.png)

4) Set the device name in the Name field.
5) Set the IP Address to e.g.) 192.168.4.150.
6) Set the Safety Network Number to e.g.) 1111_2222_3333.<br>
![CIP Safety](../../../_assets/cipSafety/Setting_SNN.png)


7) Click the Change button in Module Definition and set the Safety I/O and Standard I/O sizes.
- Standard I/O (Exclusive owner): 240 bytes
- Safety I/O: 8 bytes each
8) Do not set "Configuration signature."
9) Close the Select Module type window.<br>
![CIP Safety](../../../_assets/cipSafety/Setting_module.png)
10) Check if the module has been added.<br>
![CIP Safety](../../../_assets/cipSafety/module_added.png)
11) Press the offline button in the toolbar menu, then press the Download button.<br>
![CIP Safety](../../../_assets/cipSafety/download.png)
12) After the configured values are downloaded, change the toggle button of "Guard Logix" from PROG to RUN.
### 4) Hi7 settings (TP UI)
#### 4.1 EtherNet/IP Settings
1) Navigate to the menu: System → Control Parameters → Industrial Communication → EtherNet/IP Settings
2) Protocol setting = Adapter
3) Set the LAN port for the EtherNet/IP Adapter to LAN2.
4) Set the Input/Output size to 240 bytes each.
5) Do not change the remaining settings as shown in the figure.<br>
![CIP Safety](../../../_assets/cipSafety/ethernetIP.png)

#### 4.2 CIP Safety Settings
1) Navigate to the menu: System → Safety System → Parameter Settings → Safety Input/Output → CIP Safety.
2) Enable button ON
3) Set SNN to e.g.) 1111_2222_3333.
4) Press the Apply button.
5) Reboot the robot controller.<br>
![CIP Safety](../../../_assets/cipSafety/cipSafety_Parameters.png)
### 5 Check the communication status.
#### 5.1 EtherNet/IP
1) Check if the License LED is on.
2) Check if the Run LED is on.
3) Check if the Communication LED is on.
4) If the Error LED is on, check the Error Name.<br>
![CIP Safety](../../../_assets/cipSafety/eip_status.png)
#### 5.2 CIP Safety
1) Check if Dev status is "Executing."
2) Check if Comm status is "On-line, Connected."
3) Check if IO Count continuously increases.<br>
![CIP Safety](../../../_assets/cipSafety/cipsafety_status.png)

### 6 Safety Signal Assignment
#### 6.1 CIP Safety I/O Assignment<br>
* Refer to [3.3.3.3 Safety Signal Assignment](3-safety-function/3-safety-function/3-safety-io/3-Linker.md) page
#### 6.2 CIP Safety I/O Assignment Example
1) CIP Safety Input (Direction: Master -> Slave)
1ch(0 bit) = Arm Limit<br>
![CIP Safety](../../../_assets/cipSafety/alloc_in.png)<br>
<br> <br>
![CIP Safety](../../../_assets/cipSafety/alloc_in2.png)<br>

2) CIP Safety Output (Slave -> Master direction)
1ch(0 bit) = E-Stop Status<br>
![CIP Safety](../../../_assets/cipSafety/alloc_out.png)<br>
<br> <br>
![CIP Safety](../../../_assets/cipSafety/alloc_out2.png)<br>

