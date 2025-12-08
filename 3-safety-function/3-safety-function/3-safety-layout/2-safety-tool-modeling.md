# 3.3.2.2 Sicherheitswerkzeugmodellierung

Überwacht, ob die als Werkzeug für die Sicherheitszonenüberwachung modellierte Kugel den geschützten Bereich verletzt oder den Arbeitsbereich verlässt. Es können bis zu 16 Sicherheitswerkzeuge eingestellt und mit bis zu 10 Modellen modelliert werden.

Da das Sicherheitswerkzeug über die am Teach-Pendant eingestellte Werkzeugnummer aktiviert wird, müssen Sie das Sicherheitswerkzeug basierend auf den im Menü \[System > 3: Roboterparameter > 1: Werkzeugdaten] eingestellten Werkzeugdaten modellieren. Beziehen Sie sich auf die TCP-Positionsinformationen oben im Bildschirm für die Werkzeugdateneinstellungen.

Es gibt insgesamt drei Modelle für die Sicherheitswerkzeugmodellierung: Kugel, Kapsel und Platte. Jedes Modell besteht aus einem Mittelpunkt und einem Radius. Die Mittelpunktposition und der Radius der Modellierung werden basierend auf dem Roboterflansch-Koordinatensystem (Xf, Yf, Zf) festgelegt, und der Radius wird so eingestellt, dass er die Werkzeuggröße und den Stoppweg bei maximaler TCP-Geschwindigkeit umfasst.

<p align="center">
<img src="../../../_assets/safety_layout/tool_sphere.png"></img>
<em><p align="center">Werkzeugmodellierung</p></em>
</p>

<p align="center">
<img src="../../../_assets/safety_layout/flange.png"></img>
<em><p align="center">Roboterflansch-Koordinatensystem</p></em>
</p>

Sie können Parameterwerte im Menü **\[System > 8: Sicherheitssystem > 2: Parametereinstellung > 2: Bereichsbegrenzung > 3: Werkzeugmodellierung]** festlegen.

<p align="center">
<img src="../../../_assets/safety_layout/tool_sphere.png"></img>
<em><p align="center">Bildschirm für Modellierungseinstellungen für Sicherheitswerkzeuge</p></em>
</p>

|  **Parameter** |                       **Beschreibung**                       |  **Standardeinstellung**  |
| :-------: | :------------------------------------------------: | :----------: |
| TCP X,Y,Z | <p>TCP-Position im Flanschkoordinatensystem (schreibgeschützt) - in Werkzeuginformationen festgelegt</p> | 0 |
| Geometrie | <p>Werkzeugmodellierungsform</p><p>(aus / Kugel / Kapsel / Platte)</p> | aus |
| <p>Radius</p><p>[mm]</p> | <p>Radius</p><p>(0,0 ~ 3000,0)</p> | 0 |
| <p>Höhe</p><p>[mm]</p> | <p>Plattenhöhe</p><p>(0,0 ~ 5000,0)</p> | 0 |
| <p>Breite</p><p>[mm]</p> | <p>Plattenbreite</p><p>(0,0 ~ 5000,0)</p> | 0 |
| <p>X</p><p>[mm]</p> | <p>Modellmittelpunkt in X-Richtung</p><p>(-5000,0 ~ 5000,0)</p> | 0 |
| <p>Y</p><p>[mm]</p> | <p>Modellmittelpunkt in Y-Richtung</p><p>(-5000,0 ~ 5000,0)</p> | 0 |
| <p>Z</p><p>[mm]</p> | <p>Modellmittelpunkt in Z-Richtung</p><p>(-5000,0 ~ 5000,0)</p> | 0 |
| <p>Rot.X</p><p>[deg]</p> | <p>X-Richtung im Flanschkoordinatensystem</p><p>(-180,0 ~ 180,0)</p> | 0 |
| <p>Rot.Y</p><p>[deg]</p> | <p>Y-Richtung im Flanschkoordinatensystem</p><p>(-180,0 ~ 180,0)</p> | 0 |
| <p>Rot.Z</p><p>[deg]</p> | <p>Z-Richtung im Flanschkoordinatensystem</p><p>(-180,0 ~ 180,0)</p> | 0 |





{% hint style="warning" %}
**\[Achtung]**

* Achten Sie beim Ändern von Werkzeugdaten darauf, erneut zu überprüfen, ob die in der Sicherheitswerkzeugmodellierung eingestellten Parameter korrekt sind. Die Werkzeugdatennummer und die Sicherheitswerkzeugmodellierungsnummer desselben Werkzeugs müssen übereinstimmen.
* Da die Definition der Roboterlayout-Einstellungen nur für die Roboterachsen 2 und 3 gilt, können andere Teile des Roboters diese Zone verletzen, selbst wenn eine Sicherheitszone festgelegt ist.
{% endhint %}
