# 5.4 PROFISAFE 모니터링

`[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 6: 안전 통신 > 3: CIP Safety]` 메뉴를 선택하여 CIP Safety 입출력 상태를 모니터링 할 수 있습니다.

<p align="center">
<img src="../_assets/cipSafety/cipsafety_status.png"></img>
<em><p align="center">CIP Safety 상태 모니터링 화면</p></em>
</p>

- **장치 상태:** <br>
Executing : CIP Safety 통신 실행중. <br>
Idle : CIP Safety 프로그램 실행중이나 CIP Safety 통신 개통 전. <br>
Abort : 초기화 과정 오류<br>
Fault : 중요 오류 발생<br>
Configuring : 설정값 적용 오류<br>
- **통신 상태:**<br>
Connection Fail : 연결 실패.<br>
On-Line, Connected : Originator와 연결됨. 온라인 <br>
On-Line, No Conn : Originator와 연결되지 않음. 온라인<br>
- **입출력 카운트:** (IO 송수신 횟수)