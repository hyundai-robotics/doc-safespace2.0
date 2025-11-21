# 3.3.2.3 Sicherheitsroboter-Modellierung

Ein Robotermodell, das zur Überwachung des Sicherheitsbereichs verwendet wird. Die Sicherheitsroboter-Modellierung kann auf die Achsen 2 und 3 angewendet werden, die beide als Kapseln modelliert sind.

Die für die Sicherheitsroboter-Modellierung verwendete Kapsel besteht aus dem Mittelpunkt und dem Radius der Kugeln an beiden Enden. Der Mittelpunkt der Modellierkugel ist die Mittelposition der Roboterachse 2/3, und der Radius muss groß genug sein, um die Größe des aktuellen Glieds und den Stoppweg bei maximaler TCP-Geschwindigkeit zu berücksichtigen.

Über das Menü \[System > 4: Anwendungsparameter > 18: SafeSpace2.0 > Parametereinstellungen > Layoutbeschränkung > Roboter]* können Sie die Parameterwerte festlegen.

![Abbildung: Einstellungsbildschirm für die Modellierung von Sicherheitsrobotern](../../../_assets/safety_layout/robot_capsule.PNG)


| **| Parameter | Beschreibung | Standardeinstellung |** | 　　　　　　　　　**| Parameter | Beschreibung | Standardeinstellung |**                                     | **| Parameter | Beschreibung | Standardeinstellung |** |
| :------: | --------------------------------------------------- | :--------: |
| Radius | Kugelradius (0 bis 1000,0 (mm)) | 0 mm |
|   Model1  X,Y,Z | Kugelradius (-1000,0 bis 1000,0 (mm))                           |    0 mm    |
|   Model2 X,Y,Z | Kugelradius (-1000,0 bis 1000,0 (mm))                           |    0 mm    |

{% hint style="warning" %}
*\[Achtung]**

* Da die Definition der Roboterlayout-Einstellungen nur für die Roboterachsen 2 und 3 gilt, können andere Teile des Roboters diese Zone verletzen, selbst wenn eine Sicherheitszone festgelegt ist.
{% endhint %}