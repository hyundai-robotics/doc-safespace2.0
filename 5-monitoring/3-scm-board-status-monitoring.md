# 1.10.3 Überwachung des Status der Sicherheitsplatine

Wählen Sie das Menü **\[Einstellungen > 4: Anwendungsparameter > 21: Cobot-Setup > 1: Sicherheitsfunktion > 5: Überwachung des Sicherheitsstatus]** und dann die Registerkarte **\[SCM-Status]**, um den Status der Sicherheitsplatine zu überprüfen.

![!Abbildung 15 Cobot-Sicherheitsstatus: SCM-Status](../../_assets/image52.jpeg)

* **\[Status]**: Überprüfen Sie den Sicherheitsstatus.

  Sie können den Status der Cobot-Sicherheitsfunktionen überwachen. Bei Normalbetrieb wird **Normal** ausgegeben, und bei einem Fehler oder einer Verletzung der Sicherheitsfunktion können Sie den entsprechenden Fehlercode überprüfen.


* Überprüfen Sie den Status der Sicherheitsplatine.
  * **\[Haupt]**: SCM-Dual-MCU-Statusausgabe (MCU A, MCU B)

    POWER\_ON, INIT\_STATE, WAIT\_KIENMATICS\_INFO, WAIT\_DYNAMICS\_INFO, WAIT\_SAFE\_PARAMETER, INITIAL\_MONITORING, NORMAL\_OPERATION, , STO\_STATE\_BY\_PARAM, STO\_STATE\_BY\_SI, SS1\_STATE, SS2\_STATE, SOS\_STATE, FAULT\_STATE
  * **\[Encoder]**: Dualer Encoder-Statusausgang pro Achse (Normal, Fehler, Aus)
  * **\[Gelenkmomentensensor]**: Dualer JTS-Statusausgang pro Achse (Normal, Fehler, Aus)**: 축별 듀얼 JTS 상태 출력(Normal, Error, Off)
