# 3.3.2.3 Sicherheitsroboter-Modellierung

Ein Robotermodell, das zur Überwachung des Sicherheitsbereichs verwendet wird. Die Sicherheitsroboter-Modellierung kann auf die Achsen 2 und 3 angewendet werden, die beide als Kapseln modelliert sind.

Die für die Sicherheitsroboter-Modellierung verwendete Kapsel besteht aus dem Mittelpunkt und dem Radius der Kugeln an beiden Enden. Der Mittelpunkt der Modellierkugel ist die Mittelposition der Roboterachse 2/3, und der Radius muss groß genug sein, um die Größe des aktuellen Glieds und den Stoppweg bei maximaler TCP-Geschwindigkeit zu berücksichtigen.

Sie können Parameterwerte im Menü **\[System > 8: Sicherheitssystem > 2: Parametereinstellung > 2: Bereichsgrenzen > 2: Robotermodellierung]** festlegen.

<p align="center">
<img src="../../../_assets/safety_layout/robot_capsule.png"></img>
<em><p align="center">Bildschirm für die Modellierungseinstellungen des Sicherheitsroboters</p></em>
</p>

| **Parameter** | 　　　　　　　　　**Beschreibung**                                     | **Standardeinstellung** |
| :------: | --------------------------------------------------- | :--------: |
| <p>Höhe</p><p>[mm]</p> | <p>Plattenhöhe</p><p>(0 ~ 5000,0)</p> | 0 |
| <p>Radius</p><p>[mm]</p> | <p>Kugelradius</p><p>(0 ~ 3000,0)</p> | 10 |
| <p>Mittelpunkt</p><p>[mm]</p> | <p>Mittelpunktposition</p><p>(-3000,0 ~ 3000,0)</p> | 0 |
| <p>Richtung</p><p>[Grad]</p> | <p>Orientierung des Koordinatensystems</p><p>(-180,0 ~ 180,0)</p> | 0 |

{% hint style="warning" %}
**\*[Achtung]**

* Da die Definition der Roboterlayout-Einstellungen nur für die Roboterachsen 2 und 3 gilt, können andere Teile des Roboters diese Zone verletzen, selbst wenn eine Sicherheitszone festgelegt ist.
{% endhint %}