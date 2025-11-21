# 1.10.3 Überwachung des Status der Sicherheitsplatine

* *\[설정 > 4: 응용 파라미터 > 21: 협동로봇 설정 > 1: 안전 기능 > 5: 안전 상태 모니터링]**Wählen Sie das Menü \[Einstellungen > 4: Anwendungsparameter > 21: Cobot-Setup > 1: Sicherheitsfunktion > 5: Überwachung des Sicherheitsstatus]* und dann die Registerkarte \[SCM-Status]**, um den Status der Sicherheitsplatine zu überprüfen.**\[SCM 상태]** 탭을 선택하여 안전보드의 상태를 확인하십시오.

![!Abbildung 15 Cobot-Sicherheitsstatus: SCM-Status](../../_assets/image52.jpeg)

* **\[Status]: Überprüfen Sie den Sicherheitsstatus.**: 안전 상태를 확인합니다.

협동로봇 안전 기능의 상태를 모니터링할 수 있습니다. 정상이면 **Sie können den Status der Cobot-Sicherheitsfunktionen überwachen. Bei Normalbetrieb wird „Normal“ ausgegeben, und bei einem Fehler oder einer Verletzung der Sicherheitsfunktion können Sie den entsprechenden Fehlercode überprüfen.**이 출력되고 안전 기능 에러 또는 위반 시에는 해당 에러 코드를 확인할 수 있습니다.


* Überprüfen Sie den Status der Sicherheitsplatine.
  * **\[Haupt]: SCM-Dual-MCU-Statusausgabe (MCU A, MCU B)**: SCM의 듀얼 MCU (MCU A, MCU B) 상태 출력

POWER\_ON, INIT\_STATE, WAIT\_KIENMATICS\_INFO, WAIT\_DYNAMICS\_INFO, WAIT\_SAFE\_PARAMETER, INITIAL\_MONITORING, NORMAL\_OPERATION, , STO\_STATE\_BY\_PARAM, STO\_STATE\_BY\_SI, SS1\_STATE, SS2\_STATE, SOS\_STATE, FAULT\_STATE
  * **\[Encoder]: Dualer Encoder-Statusausgang pro Achse (Normal, Fehler, Aus)**: 축별 듀얼 엔코더 상태 출력(Normal, Error, Off)
  * **\[Gelenkmomentensensor]: Dualer JTS-Statusausgang pro Achse (Normal, Fehler, Aus)**: 축별 듀얼 JTS 상태 출력(Normal, Error, Off)
