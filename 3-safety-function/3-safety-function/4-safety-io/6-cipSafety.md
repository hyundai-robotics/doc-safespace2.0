

# 3.3.4.6 CIP Safety

### 1. CIP Safety ?
- CIP Safety는 표준 Common Industrial Protocol(CIP)을 확장한 안전 통신 프로토콜
- '블랙 채널' 원리를 사용하여 EtherNet/IP 및 DeviceNet 상에서 안전한 데이터 교환을 가능하게 함.
- 시간 감시, 이중화, CRC 검사 등의 메커니즘을 통해 IEC 61508, ISO 13849 등의 안전 표준을 준수함.

### 2. 사양
#### 2.1 EtherNet/IP
- 디지털 입력 : 0 ~ 240 bytes
- 디지털 출력 : 0 ~ 240 bytes
- 통신 주기 : 5 ~ 3000 msec
- 지원 통신 속도 : 10 or 100 Mbps

#### 2.2 CIP Safety
- 안전 입출력 : 8/8 bytes 
- 통신 주기 : 20 ~ 100 msec


### 3. CIP Safety 파라미터
`[시스템 > 2: 제어 파라미터 > 11:산업용 통신 > 6: 안전 통신 > 3: CIP Safety]`<br>
![](../../../_assets/cipSafety/cipSafety_Parameters.png)

 - 안전 네트워크 번호 : Safety Network Number를 설정 합니다.
 - IP 주소 : 현재 EtherNet/IP Adapter의 설정된 IP 주소를 표시합니다.
{% hint style="info" %}
* EtherNet/IP Adapter의 IP가 변경된 경우에는 반드시 CIP Safety 파라미터의 전체적용을 실행해 주십시오.
{% endhint %}
 
   

### 4. CIP Safety 설정 절차

1) Hi7 EtherNet/IP Adapter와 EtherNet/IP Scanner의 연결
2) 엔지니어링 툴을 통한 EDS 파일 추가(Studio 5000)
3) CIP Safety 컨트롤러 설정 (Studio 5000)
4) Hi7 설정 (TP UI)
4.1) EtherNet/IP 설정
4.2) CIP Safety 설정
5) EtherNet/IP와 CIP Safety 통신 상태 확인
6) 안전 신호의 할당


#### 1 Hi7 EtherNet/IP Adapter와 EtherNet/IP Scanner의 연결
![](../../../_assets/cipSafety/connect.png)

#### 2 엔지니어링 툴을 통한 EDS 파일 추가(Studio 5000)
- 'Device Description File Installation Tool'을 사용하여 EDS(Hi7_EIP_251023.eds)파일을 설치합니다.
#### 3 CIP Safety 컨트롤러 설정 (Studio 5000)
1) Studio 5000을 실행하고 새 프로젝트를 만듭니다.
2) controller organizer에서 CIP Safety 통신을 지원하는 컨트롤러(예 CPU 1769-L30ERMS)를 선택하고 Ethernet을 선택한뒤 마우스 우측버튼을 눌러 New Module을 클릭합니다.
3) "Hi7 EIP Adapter"를 찾고 Create 버튼을 누릅니다.<br>
![CIP Safety](../../../_assets/cipSafety/new_module.png)

4) Name칸에 장치의 이름을 설정합니다.
5) IP Address는 예)192.168.4.150으로 설정합니다.
6) Safety Network Number는 예)1111_2222_3333으로 설정합니다.<br>
![CIP Safety](../../../_assets/cipSafety/Setting_SNN.png)


7) Module Definition에서 Change 버튼 클릭후 Safety I/O 와 표준 I/O 크기를 설정합니다.
- Standard I/O(Exclusive owner) : 240 bytes
- Safety I/O : 각각 8 bytes
8) "Configuration signature" 설정하지 마십시오.
9) Select Module type 창을 닫으세요.<br>
![CIP Safety](../../../_assets/cipSafety/Setting_module.png)
10) 모듈이 추가되었는지 확인하세요<br>
![CIP Safety](../../../_assets/cipSafety/module_added.png)
11) 툴바 메뉴에서 offline 버튼을 눌러 Download 버튼을 누르세요.<br>
![CIP Safety](../../../_assets/cipSafety/download.png)
12) 설정한 값들이 다운로드 된 후 "Guard Logix"의 토글 버튼을 PROG 에서 RUN으로 바꾸세요.
#### 4 Hi7 설정 (TP UI)
##### 4.1 EtherNet/IP 설정
1) 시스템 → 제어 파라미터 → 산업용 통신 → EtherNet/IP 설정으로 메뉴 이동
2) Protocol 설정 = Adapter
3) EtherNet/IP Adapter를 위한 랜포트 설정은 LAN2로 설정합니다.
4) Input/Output 사이즈는 각각 240 바이트로 설정합니다.
5) 나머지 설정은 그림과 같이 변경하지 않습니다.<br>
![CIP Safety](../../../_assets/cipSafety/ethernetIP.png)

##### 4.2 CIP Safety 설정
1) `시스템 → 2:제어 파라미터 -> 11:산업용 통신 -> 6:안전 통신 → 3: CIP Safety`로 메뉴 이동합니다.
2) 활성화 버튼 ON
3) SNN 예)1111_2222_3333으로 설정합니다.
4) 적용 버튼 누릅니다.
5) 로봇 제어기를 재부팅 합니다.<br>
![CIP Safety](../../../_assets/cipSafety/cipSafety_Parameters.png)
#### 5 통신 상태 확인
##### 5.1 EtherNet/IP
1) License Led 점등 확인
2) Run Led is 점등 확인
3) Communication Led 점등 확인
4) Error Led가 점등된 경우 Error Name을 확인<br>
![CIP Safety](../../../_assets/cipSafety/eip_status.png)
##### 5.2 CIP Safety
1) 안전 통신 선택이 "CIP Safety"인지 확인
2) Comm status가 "On-line, Connected" 상태인지 확인
3) IO Count가 지속 증가하는지 확인<br>
![CIP Safety](../../../_assets/cipSafety/cipsafety_status.png)

#### 6 안전 신호의 할당
##### 6.1 CIP Safety 입출력의 할당<br>
* [3.3.4.3 안전 신호 할당](../4-safety-io/3-Linker.md) 페이지 참고
##### 6.2 CIP Safety 입출력 할당의 예
1) CIP Safety Input (Master -> Slave 방향)
1ch(0 bit) = Arm Limit<br>
![CIP Safety](../../../_assets/cipSafety/alloc_in.png)<br>
<br> <br>
![CIP Safety](../../../_assets/cipSafety/alloc_in2.png)<br>

2) CIP Safety Output (Slave -> Master 방향)
1ch(0 bit) = E-Stop Status<br>
![CIP Safety](../../../_assets/cipSafety/alloc_out.png)<br>
<br> <br>
![CIP Safety](../../../_assets/cipSafety/alloc_out2.png)<br>

