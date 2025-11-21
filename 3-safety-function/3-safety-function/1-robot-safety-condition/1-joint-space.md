# 3.3.1.1 Einstellung der Gelenkwinkelgrenzen

Gelenkgrenzenparameter sind Schwellenwerte zur Überwachung der Sicherheitsfunktionen im Gelenkraum des Roboters. Bei einer Verletzung der Überwachung wird sofort der eingestellte Sicherheitshalt ( Stopp 0, Stopp 1, Stopp 2) aktiviert.

![!Abbildung 4 Beispiel für die Einstellung der Gelenkwinkelgrenze (S-Achse)](<../../../_assets/joint_space.png>)

Über das Menü \[System > 4: Anwendungsparameter > 18: SafeSpace2.0 > Parametereinstellungen > Roboterbeschränkung > Gelenkwinkelgrenze]* können Sie Parameterwerte festlegen.

![!Abbildung 5 Bildschirm zur Einstellung der Gelenkwinkelgrenzenparameter](<../../../_assets/joint_space_param.png>)

|  **| Parameter | Beschreibung | Standardeinstellung |** |                       **| Parameter | Beschreibung | Standardeinstellung |**                       |  **| Parameter | Beschreibung | Standardeinstellung |**  |
| :-------: | :------------------------------------------------: | :----------: |
| Type |  <p>Sicherheitszonentyp</p><p>(Arbeitsbereich/geschützter Bereich)</p>  | Arbeitsbereich|
| Activation | <p>Funktionsaktivierungsstatus</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stoppmethode bei Funktionsverletzung</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Joint OnOff |   <p>Aktivierungsstatus jedes Gelenks</p><p>(On/Off)</p>  |  Off |
| Min |   <p>Winkelgrenzwert für jedes Gelenk</p><p>(-360.0 ~ 360.0 (deg))</p>  |  -360.0 |
| Max |   <p>Winkelgrenzwert für jedes Gelenk</p><p>(-360.0 ~ 360.0 (deg))</p>  |  360.0 |

{% hint style="warning" %}
*\[Achtung]**: Die Sicherheitsfunktion überwacht basierend auf der eingestellten Zone. Die eingestellte Zone muss unter Berücksichtigung des Stoppwegs konfiguriert und vor dem Betrieb überprüft werden.
{% endhint %}
 