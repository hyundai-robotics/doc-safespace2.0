

# 3.3.3.5 PROFIsafe

 **1. PROFIsafe settings**

![Profisafe Consol Image](../../../_assets/safetyio_profisafe/BD671_console.png)

 - Source Address : Set the source Address. (fixed to 1)
 - Destination Address : Set the destination Address. (Setting range : 1 ~ 65534)
 
  **2. Notes** 
  
 - Address Type :  Address Type 1 (Check Destination Address only)
 - Reaction on Device_Fault : When this device enters a Fault state, all F-Output will be changed to Fail-safe (0) status. After resolving the device's Fault state, a process of reintegrating the F-Device is necessary from the F-Host using commands such as Global Acknowledge.
 
 **3. 알람 리스트** 

|Alarm No.|Alarm Decsription  | 
|--|--|
| 0x10 |Parameter setting error |
| 0x13 |Communication error|
| 0x19 |Safety function error |
| 0x1C |Internal communication error 1 |
| 0x1D |Internal communication error 2 |
| 0x1E |Internal communication error 3 |
| 0x40 |F-Dest Address setting error |
| 0x41 |F-Dest Address value is invalid |
| 0x42 |F-Src Address setting error |
| 0x43 |F-Watchdog value is invalid
| 0x45 |F-CRC length is invalid |
| 0x46 |F-PAR version is invalid |
| 0x47 |CRC1 is invalid |
| 0x4C |F-Block ID is invalid |
| 0x4D |CRC2 is invalid|
| 0x4E |F-Watchdog timeout|


> Parameter settings using the TP below are in preparation.

![Profisafe TP Image](../../../_assets/safetyio_profisafe/profisafe.PNG)

 - Source Address : Set the source Address. (1로 고정)
 - Destination Address : Set the destination Address. (Setting range : 1 ~ 65534)
