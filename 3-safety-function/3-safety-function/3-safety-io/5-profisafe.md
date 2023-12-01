

# 3.3.3.5 PROFIsafe

 **1. PROFIsafe의 설정**

![Profisafe Consol Image](../../../_assets/safetyio_profisafe/BD671_console.png)

 - Source Address : Source Address를 설정합니다. (설정 범위 : 1 ~ 65534)
 - Destination Address : Destination Address를 설정합니다. (설정 범위 : 1 ~ 65534)
 
  **2. 참고 사항** 
  
 - Address Type :  Address Type 2 (Source & Destination Address 모두 체크함)
 - Reaction on Device_Fault : 본 장치가 Fault 상태가 되면 모든 F-Output 출력은 Fail-safe(0)상태로 변경됩니다. 그리고 장치의 Fault상태가 해소되고 난 뒤에는 F-Host에서 Global- Acknowledge 와 같은 명령으로 F-Device를 re-integration 하는 과정이 필요합니다.
 
 **3. 알람 리스트** 

|Alarm No.|Alarm Decsription  | 
|--|--|
| 0x10 |파라미터 설정 오류 |
| 0x13 |통신 오류|
| 0x19 |안전기능 오류 |
| 0x1C |내부통신 오류1 |
| 0x1D |내부통신 오류2 |
| 0x1E |내부통신 오류3 |
| 0x40 |F-Dest Address 설정 오류 |
| 0x41 |F-Dest Address 값이 유효하지 않음 |
| 0x42 |F-Src Address 설정 오류 |
| 0x43 |F-Watchdog 값이 유효하지 않음
| 0x45 |F-CRC 길이 이상 |
| 0x46 |F-PAR 버젼 이상 |
| 0x47 |CRC1 이상 |
| 0x4C |F-Block ID 이상 |
| 0x4D |CRC2 이상|
| 0x4E |F-Watchdog 타임아웃|


> 아래 TP에 의한 파라미터 설정은 준비중에 있습니다.

![Profisafe TP Image](../../../_assets/safetyio_profisafe/profisafe.PNG)

 - Source Address : Source Address를 설정합니다. (설정 범위 : 1 ~ 65534)
 - Destination Address : Destination Address를 설정합니다. (설정 범위 : 1 ~ 65534)
