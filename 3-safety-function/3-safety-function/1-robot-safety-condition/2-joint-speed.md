# 3.3.1.2 Gelenkgeschwindigkeitsgrenze

Die Parameter für die Gelenkgeschwindigkeitsgrenze sind Schwellenwerte zur Überwachung der Gelenkgeschwindigkeit des Roboters. Bei Verletzung des Schwellenwerts wird sofort der eingestellte Sicherheitsstopp (Stopp 0, Stopp 1, Stopp 2) aktiviert.

![!Abbildung 4 Beispiel für die Einstellung der Gelenkgeschwindigkeitsgrenze](../../../_assets/joint_speed.png)

Über das Menü \[System > 4: Anwendungsparameter > 18: SafeSpace2.0 > Parametereinstellungen > Roboterbeschränkung > Gelenkgeschwindigkeitsgrenze]* können Sie die Parameterwerte festlegen.

![!Abbildung 5 Bildschirm zur Einstellung der Parameter für die Gelenkgeschwindigkeitsgrenze](<../../../_assets/joint_speed_param.png>)

|  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |** |                       **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**                       |  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Funktionsaktivierungsstatus</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stoppmethode bei Funktionsverletzung</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Joint OnOff |   <p>Aktivierungsstatus jedes Gelenks</p><p>(On/Off)</p>  |  Off |
| speed |   <p>Geschwindigkeitsbegrenzungswert für jedes Gelenk</p><p>(0 ~ 5000 (mm/s))</p>  |  5000.0 |

{% hint style="warning" %}
*\[Achtung]**: Berücksichtigen Sie bei der Einstellung der Geschwindigkeitsüberwachungsfunktion unbedingt die Stopp-Reaktionszeit und die Abdeckung, um Kollisionen und Verletzungen zu vermeiden.
{% endhint %}
 
