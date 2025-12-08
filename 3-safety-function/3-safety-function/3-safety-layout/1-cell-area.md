# 3.3.3.1 Einstellung der Sicherheitszone

Eine Sicherheitszone ist ein Arbeitsbereich oder geschützter Bereich zur Überwachung des Werkzeugs und der Robotergliederbereiche. Der Arbeitsbereich ist ein begrenzter Bereich, in dem sich das überwachte Objekt frei bewegen kann, aber nicht verlassen darf. Im Gegensatz dazu ist der geschützte Bereich ein begrenzter Raum, in dem sich das überwachte Objekt nach dem Betreten nicht mehr bewegen kann. Wenn der Roboter den festgelegten Arbeitsbereich verlässt oder in den geschützten Bereich eindringt, wird ein Sicherheitsstopp (Stopp 0, Stopp 1, Stopp 2) ausgelöst.

<p align="center">
<img src="../../../_assets/safety_layout/cell_working.png"></img>
<em><p align="center">Arbeitsraum</p></em>
</p>

<p align="center">
<img src="../../../_assets/safety_layout/cell_protected.png"></img>
<em><p align="center">geschützter Raum</p></em>
</p>

Die Sicherheitszone wird durch Festlegen der Position und Höhe jedes Eckpunkts relativ zum Koordinatensystem des Roboters konfiguriert. Es können bis zu 10 Eckpunkte hinzugefügt werden. Die Sicherheitszone wird durch Parametereinstellungen oder Sicherheits-Ein-/Ausgangssignale aktiviert.

Die Parameterwerte für die Sicherheitszone können Sie auf jeder Registerkarte des Menüs **\[System > 8: Sicherheitssystem > 2: Parametereinstellung > 2: Zonenbegrenzung > 1: Zone]** festlegen.


* **allgemein**

<p align="center">
<img src="../../../_assets/safety_layout/cell_general.png"></img>
<em><p align="center">allgemein</p></em>
</p>

|  **Parameter** |                       **Beschreibung**                       |  **Standardeinstellung**  |
| :-------: | :------------------------------------------------: | :----------: |
| Aktivierung | <p>Funktionsaktivierungsstatus</p><p>(Ein-/Aus-/Sicherheitseingang)</p> |   aus  |
| Stoppfunktion |   <p>Stoppmethode bei Funktionsverletzung</p><p>(Stopp 0, Stopp 1, Stopp 2, Nicht-Stopp)</p>  | Stopp 1 |
| Typ |  <p>Sicherheitszonentyp</p><p>(Arbeitsbereich/geschützter Bereich)</p>  | Arbeitsbereich|


* **Erkennungsziel**

<p align="center">
<img src="../../../_assets/safety_layout/cell_target.png"></img>
<em><p align="center">Erkennungsziel</p></em>
</p>

|  **Parameter** |                       **Beschreibung**                       |  **Standardeinstellung**  |
| :-------: | :------------------------------------------------: | :----------: |
| Werkzeug | <p>Überwachung der Werkzeugmodellierung</p><p>(Ein-/Aus-/Sicherheitseingang)</p> |   Aus  |
| Unterarm |   <p>Überwachung der Modellierung der Roboterachse 2</p><p>(Aus/Ein)</p>  | Aus |
| Oberarm |  <p>Überwachung der Modellierung der Roboterachse 3</p><p>(Aus/Ein)</p>  | Aus |


* **Bereich**

<p align="center">
<img src="../../../_assets/safety_layout/cell_working.png"></img>
<em><p align="center">Bereich</p></em>
</p>

|  **Parameter** |                       **Beschreibung**                       |  **Standardeinstellung**  |
| :-------: | :------------------------------------------------: | :----------: |
| <p>Z Min / Max</p><p>[mm]</p> | <p>Höhe des Sicherheitsbereichs basierend auf dem Roboterkoordinatensystem</p><p>(-5000,0 ~ 5000,0)</p> | 0 |
| Aktivieren | <p>Schwellenwert des Sicherheitsbereichs aktivieren</p><p>(Aktivieren / Deaktivieren)</p> | Deaktivieren |
| <p>X</p><p>[mm]</p> | <p>Position des Schwellenwerts in X-Richtung basierend auf dem Roboterkoordinatensystem</p><p>(-5000,0 ~ 5000,0)</p> | 0 |
| <p>Y</p><p>[mm]</p> | <p>Position des Schwellenwerts in Y-Richtung basierend auf dem Roboterkoordinatensystem</p><p>(-5000,0 ~ 5000,0)</p> | 0 |



{% hint style="warning" %}
**\[Achtung]**: Die Sicherheitsfunktion überwacht basierend auf der eingestellten Zone. Die eingestellte Zone muss unter Berücksichtigung des Stoppwegs konfiguriert und vor dem Betrieb überprüft werden.
{% endhint %}