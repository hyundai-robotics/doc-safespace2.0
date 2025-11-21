# 3.3.2.1 Einstellung der Sicherheitszone

Eine Sicherheitszone ist ein Arbeitsbereich oder geschützter Bereich zur Überwachung des Werkzeugs und der Robotergliederbereiche. Der Arbeitsbereich ist ein begrenzter Bereich, in dem sich das überwachte Objekt frei bewegen kann, aber nicht verlassen darf. Im Gegensatz dazu ist der geschützte Bereich ein begrenzter Raum, in dem sich das überwachte Objekt nach dem Betreten nicht mehr bewegen kann. Wenn der Roboter den festgelegten Arbeitsbereich verlässt oder in den geschützten Bereich eindringt, wird ein Sicherheitsstopp (Stopp 0, Stopp 1, Stopp 2) ausgelöst.

![!Arbeitsbereich](<../../../_assets/safety_layout/cell_working.PNG>)

![!Geschützter Bereich](<../../../_assets/safety_layout/cell_protected.PNG>)

Die Sicherheitszone wird durch Festlegen der Position und Höhe jedes Eckpunktes auf der Grundlage des Roboterkoordinatensystems konfiguriert. Es können bis zu 10 Eckpunkte hinzugefügt werden. Der Sicherheitsbereich wird durch Parametereinstellungen oder Sicherheits-E/A-Signale aktiviert.

안전 영역은 **Sicherheitszonen können durch Einstellen der Parameterwerte in den einzelnen Registerkarten des Menüs \[System > 4: Anwendungsparameter > 18: SafeSpace2.0 > Parametereinstellungen > Layoutbeschränkung > Zellbereich] konfiguriert werden.** 메뉴의 각 탭에서 파라미터값을 설정할 수 있습니다.


* **General**
![](../../../_assets/safety_layout/cell_general.PNG)

|  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |** |                       **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**                       |  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Funktionsaktivierungsstatus</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stoppmethode bei Funktionsverletzung</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Type |  <p>Sicherheitszonentyp</p><p>(Arbeitsbereich/geschützter Bereich)</p>  | Arbeitsbereich|


* **Target**
![](../../../_assets/safety_layout/cell_target.PNG)

|  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |** |                       **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**                       |  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**  |
| :-------: | :------------------------------------------------: | :----------: |
| Tool | <p>Überwachung der Werkzeugmodellierung</p><p>(Off/On/Safety Input)</p> |   Off  |
| Lower arm |   <p>Überwachung der Modellierung der Roboterachse 2</p><p>(Off/On)</p>  | Off |
| Upper arm |  <p>Überwachung der Modellierung der Roboterachse 3</p><p>(Off/On)</p>  | Off |


* **Area**
![](../../../_assets/safety_layout/cell_working.PNG)

|  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |** |                       **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**                       |  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**  |
| :-------: | :------------------------------------------------: | :----------: |
| Z min/max | <p>Höhe der Sicherheitszone basierend auf dem Roboterkoordinatensystem</p><p>(-5000.0 ~ 5000.0 mm)</p> |   0  |
| Vertex OnnOff |   <p>Aktivierungsstatus der Eckpunkte der Sicherheitszone</p><p>(Off/On)</p>  | Off |
| X |  <p>Position des Eckpunkts in X-Richtung basierend auf dem Roboterkoordinatensystem</p><p>(-5000.0 ~ 5000.0 mm)</p>  | 0 |
| Y |  <p>Position des Eckpunkts in Y-Richtung basierend auf dem Roboterkoordinatensystem</p><p>(-5000.0 ~ 5000.0 mm)</p>  | 0 |








{% hint style="warning" %}
*\[Achtung]**: Die Sicherheitsfunktion überwacht basierend auf der eingestellten Zone. Die eingestellte Zone muss unter Berücksichtigung des Stoppwegs konfiguriert und vor dem Betrieb überprüft werden.
{% endhint %}