# 3.3.2.1 Einstellung der Gelenkwinkelgrenzen

Der Parameter „Gelenkbereichseinstellung“ ist ein Grenzwert zur Überwachung der Sicherheitsfunktionen im Gelenkraum des Roboters. Wird die Überwachung überschritten, wird der festgelegte Sicherheitsstopp (Stop 0, Stopp 1 oder Stopp 2) sofort aktiviert.

<p align="center">
<img src="../../../_assets/joint_space.PNG"></img>
<em><p align="center">Beispiel für die Einstellung des Gelenkbereichs (S-Achse)</p></em>
</p>

Sie können Parameterwerte im Menü **\[System > 8: Sicherheitssystem > 2: Parametereinstellungen > 1: Robotergrenzen > 1: Gelenkbereich]** festlegen.

<p align="center">
<img src="../../../_assets/joint_space_param.png"></img>
<em><p align="center">Bildschirm zur Einstellung der Gelenkbereichsparameter</p></em>
</p>


|  **Parameter** |                       **Beschreibung**                       |  **Standardeinstellung**  |
| :-------: | :------------------------------------------------: | :----------: |
| Typ | <p>Sicherheitsbereichstyp</p><p>(Arbeitsbereich / Schutzbereich)</p> | Arbeitsbereich |
| Aktivierung | <p>Funktion aktiviert</p><p>(Ungültig / Gültig / Sichere E/A)</p> | Ungültig |
| Stoppmethode | <p>Stoppmethode bei Funktionsverletzung</p><p>(Stop 0 / Stopp 1 / Stopp 2 / Kein Stopp)</p> | Stopp 1 |
| Gelenkaktivierung | <p>Aktiviert jedes Gelenk</p><p>(Aktiv / Inaktiv)</p> | Inaktiv |
| <p>Minimum</p><p>[Grad]</p> | <p>Winkelgrenzwert für jedes Gelenk</p><p>(-360,0 ~ 360,0)</p> | -360,0 |
| <p>Maximum</p><p>[Grad]</p> | <p>Winkelgrenzen für jedes Gelenk</p><p>(-360,0 ~ 360,0)</p> | 360,0 |

{% hint style="warning" %}
*\[Achtung]**: Die Sicherheitsfunktion überwacht basierend auf der eingestellten Zone. Die eingestellte Zone muss unter Berücksichtigung des Stoppwegs konfiguriert und vor dem Betrieb überprüft werden.
{% endhint %}
 