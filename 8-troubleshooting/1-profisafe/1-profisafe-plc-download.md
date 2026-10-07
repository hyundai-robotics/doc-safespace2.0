# Case 1 - PLC S/W Download 후 PROFIsafe 통신이 복구되지 않는 경우

## 1) 발생 상황
PROFIsafe(PROFINET) 통신이 정상인 상태에서 PLC 소프트웨어(Ladder 또는 통신 설정)를 변경하고 PLC S/W Download를 수행한 경우

## 2) 발생 원인 및 조치 방법

PLC S/W Download를 수행하는 과정에서 PLC와 Hi7 간 PROFIsafe(PROFINET) 통신이 일시적으로 끊길 수 있습니다. 이 경우 아래와 같은 알람이 발생할 수 있습니다.

- E52202 PROFINET 단선 알람
- E52306 F-Watchdog 알람

대부분 PLC 소프트웨어의 Download가 완료되고 PLC가 재시작되면 모든 알람이 클리어되고 통신이 정상 상태로 복구됩니다.

간혹 PROFINET 관련 알람이 클리어되지 않는 경우에는 **[모터 ON] 동작**을 통해 해당 알람을 클리어할 수 있습니다.

단, PROFIsafe 통신의 경우 PROFINET 통신이 정상적으로 복구되더라도 **[ACK_GL] Function Block을 통한 Re-integration 과정이 반드시 필요**합니다.

자세한 방법은 아래 조치 절차를 참조하십시오.

## 3) 조치 절차

### Step 1) 알람 클리어
- `[Shift] + [Mot.ON]` 버튼을 눌러 알람을 클리어한다.<br>
(※ V70.04-00 이후: PROFINET 통신 재연결 시 알람 자동 클리어 됨)

<p align="center">
<img src="../../_assets/trouble/keys_moton.png"></img>
</p>

### Step 2) PROFINET 통신 상태 확인
- `[시스템]` → `[제어 파라미터]` → `[산업용 통신]`  → `[프로피넷 설정]` 화면에서 통신 상태를 확인한다.

아래 그림과 같이 설정된 모든 슬롯의 상태가 **GOOD** 이어야 하고 카운터는 모두 증가 상태여야 한다. 그렇지 않은 경우 **장치 이름**, **슬롯 설정**, **통신 케이블**의 상태를 점검한다.

<p align="center">
<img src="../../_assets/trouble/profinet_config.png"></img>
</p>

### Step 3) Safety 모듈 에러 잔존 시

- **ACK-GL의 ACK_GLOB에 라이징에지 입력 기능을 사용하여 Safety 모듈 에러를 해제한다.**
( 아래 4) Ladder 프로그램 예 참조 )

PROFINET 통신이 정상적으로 복구된 뒤 PROFIsafe 통신이 **Re-integration** 절차가 필요한 경우 화면

<p align="center">
<img src="../../_assets/trouble/tia_portal_project_bad.png"></img>
<br>[프로젝트 트리 화면]
</p>

<p align="center">
<img src="../../_assets/trouble/tia_portal_project_dev_overview.png"></img>
<br>[장치 화면]
</p>

<p align="center">
<img src="../../_assets/trouble/profisafe_config.png"></img>
<br>[PROFIsafe 설정 화면]
</p>

FappState : Cycle_DATA_EX<br>
F-Parameter : OK<br>
Config : OK<br>
IO Count : Input(왼쪽 증가) / **Output(변화 없음)**<br>




## 4) Ladder 프로그램 예

- Safety Ladder 구현 예 참조

Network 1 : PROFIsafe 입력(Hi7 -> PLC) 0번 비트 사용 <br>
Network 2 : PROFIsafe 출력(PLC -> Hi7) 0번 비트 사용 <br>
Network 3 : **ACK_GL** (ACK_GLOB에 라이징에지 입력 넣어 Re-integration 과정 수행)<br>

<p align="center">
<img src="../../_assets/trouble/device_overview-address.png"></img>
<br>[IO 주소 확인]
</p>

<p align="center">
<img src="../../_assets/trouble/simple_ladder.png"></img>
<br>[Sample Ladder]
</p>