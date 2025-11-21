# 3.3.1.9 Sicherheitsstoppfunktion

Legen Sie für jede Sicherheitsfunktion den geeigneten Sicherheitsstopp-Typ fest. Die Sicherheitsstoppfunktion stoppt den Roboter, um einen sicheren Zustand herzustellen, wenn die Sicherheit verletzt wird. Es gibt drei Arten von Sicherheitsstoppfunktionen. Alle Kategorien von Sicherheitsstoppfunktionen erfüllen die Anforderungen von 4.2.2.4 der Norm IEC 61800-5-2.

* **Stopp 0: Sofortige Unterbrechung der Stromversorgung aller Gelenkmodule und Stopp.**: 모든 조인트 모듈의 모터 전원을 즉시 제거하고 정지
* **Stopp 1: Die Motoren aller Gelenkmodule werden abgebremst und gestoppt. Anschließend wird die Stromversorgung unterbrochen.**: 모든 조인트 모듈의 모터가 감속 후 정지. 이후에 모터의 전원 제거
* **Stopp 2: Die Motoren aller Gelenkmodule werden abgebremst, anschließend wird ein sicherer Betriebshalt („Safe Operating Stop“, SOS) ausgelöst. Die Stromversorgung aller Motoren wird aufrechterhalten.**: 모든 조인트 모듈의 모터가 감속 후 SOS (Safe Operating Stop)가 동작. 모든 모터의 전원 공급 유지 상태

Der Stopptyp für Stopps aufgrund von Verstößen gegen Sicherheitsfunktionen wird im Parametereinstellungsmenü für jede Funktion festgelegt.
Die Stopptyp-Einstellungen für Stopps, die gemäß ISO 10218-1 erforderlich sind, lauten wie folgt:

Über das Menü \[System > 4: Anwendungsparameter > 18: SafeSpace2.0 > Allgemeine Einstellungen > Sicherheitshalt]* können Sie die Parameterwerte festlegen.

![](../../../_assets/safety_stop.PNG)

|  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |** |                       **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**                       |  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**  |
| :-------: | :------------------------------------------------: | :----------: |
| EM stop |  <p>Not-Halt</p><p>(Stop 0, Stop 1)</p>  | Stop 0 |
| Protective stop | <p>Sicherheitshalt</p><p>(Stop 0, Stop 1, Stop 2)</p> |   Stop 0 |
| Normal stop |   <p>Normalhalt</p><p>(Stop 0, Stop 1)</p>  | Stop 0 |
| Manual stop |   <p>Stopp, wenn die Geschwindigkeit im manuellen Modus überschritten wird</p><p>(Stop 0, Stop 1)</p>  |  Stop 0 |


{% hint style="warning" %}
*\[Achtung]**: Sie müssen für jede Funktion nach einer Risikobewertung eine geeignete Stoppmethode festlegen.
{% endhint %}
