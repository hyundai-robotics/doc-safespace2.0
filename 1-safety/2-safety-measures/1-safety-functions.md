# 1.2.1 안전 기능

## SafeSpace2.0 안전기능
SafeSpace2.0은 다음의 안전 기능을 기반으로 로봇의 위치/속도/방향 등을 감시하여 위반 상황 발생시 로봇을 정지시킬 수 있습니다. 또한, 협동 작업을 수행할 수 있는 안전 기능을 제공합니다. 각 안전 기능에 대한 자세한 내용은 "[3. SafeSpace2.0 안전 기능](../../3-safety-function/README.md)" 을 참조하십시오.

* 안전 토크 정지(STO: Safe Torque Off)
* 안전 정지1 (SS1: Safe Stop 1)
* 안전 정지2 (SS2: Safe Stop 2)
* 비상 정지(EM Stop, Emergency Stop)
* 보호 정지(Protective Stop)
* 일반 정지(Normal stop)
* 축 정지 감시(SOS: Safe Opertaing Stop)
* 정지 시간 감시(Stopping time Monitoring)
* 정지 거리 감시(Stopping distance Monitoring)
* 조인트 각도 감시(Joint-SLP, Joint Angle Monitoring)
* 조인트 속도 감시(Joint-SLS, Joint Angular Speed Monitoring)
* TCP 위치 감시(TCP-SLP, TCP Position Monitoring)
* TCP 방향 감시(TCP Orientation Monitoring)
* TCP 속도 감시(TCP-SLS, TCP Speed Monitoring)
* 파워 감시(Power Monitoring)
* 모멘텀 감시(Momentum Monitoring)
* 충돌 검지(Collision Detection)
* 속도 및 이격 거리 감시(Speed and Seperation Monitoring)
* 안전 브레이크 제어(SBC: Safe Brake Control)
* 안전 입력(Safety Inputs)
* 안전 출력(Safety Outputs)
* PROFIsafe
* 시작/재시작 인터록(Start/restart Interlock)


---


## 옵션 라이선스
SafeSpace2.0은 총 3가지의 옵션 라이선스를 제공합니다. 라이선스에 따라 사용할 수 있는 기능 사양이 다릅니다. 자세한 것을 아래 표를 참고하십시오. 

|  **안전 기능** |                       **기본 제공**                       |  **옵션 1 (베이직)**  |  **옵션 2 (프로)**  |  **옵션 3 (협동)**  |
| :-------: | :------------------------------------------------: | :----------: | :----------: | :----------: |
| 비상정지/보호정지(SGG,SGA) |  O  | O | O | O |
| 수동모드 속도 감시 |  O  | O | O | O |
| 정지거리/정지시간 감시 |  O  | O | O | O |
| 축 위치 감시 |    | O | O | O |
| TCP 위치 감시 |    | O | O | O |
| TCP 감시 영역 |    | 1개 | 16개 | 16개 |
| 축 속도 감시 |    |  | O | O |
| TCP 속도 감시 |    |  | O | O |
| TCP 방향 감시 |    |  | O | O |
| 축 정지 감시 |    |  | O | O |
| 자가 충돌 감시 |    |  | O | O |
| 속도 및 이격 거리 감시 |    |  | O | O |
| 충돌/파워/모멘텀 감시 |    |  |  | O |
| 안전 모션 |    |  |  | O |
