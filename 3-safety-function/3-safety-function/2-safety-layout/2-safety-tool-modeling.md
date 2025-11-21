# 3.3.2.2 Sicherheitswerkzeugmodellierung

Überwacht, ob die als Werkzeug für die Sicherheitszonenüberwachung modellierte Kugel den geschützten Bereich verletzt oder den Arbeitsbereich verlässt. Es können bis zu 16 Sicherheitswerkzeuge eingestellt und mit bis zu 10 Modellen modelliert werden.

Da das Sicherheitswerkzeug über die am Teach-Pendant eingestellte Werkzeugnummer aktiviert wird, müssen Sie das Sicherheitswerkzeug basierend auf den im Menü \[Einstellungen > 3: Roboterparameter > 1: Werkzeugdaten] eingestellten Werkzeugdaten modellieren. Beziehen Sie sich auf die TCP-Positionsinformationen oben im Bildschirm für die Werkzeugdateneinstellungen.

Es gibt insgesamt drei Modelle für die Sicherheitswerkzeugmodellierung: Kugel, Kapsel und Platte. Jedes Modell besteht aus einem Mittelpunkt und einem Radius. Die Mittelpunktposition und der Radius der Modellierung werden basierend auf dem Roboterflansch-Koordinatensystem (Xf, Yf, Zf) festgelegt, und der Radius wird so eingestellt, dass er die Werkzeuggröße und den Stoppweg bei maximaler TCP-Geschwindigkeit umfasst.

![!Abbildung Werkzeugmodellierung](../../../_assets/safety_layout/tool_sphere.PNG)

![!Abbildung Roboterflansch-Koordinatensystem](../../../_assets/safety_layout/flange.PNG)


Über das Menü \[System > 4: Anwendungsparameter > 18: SafeSpace2.0 > Parametereinstellungen > Layoutbeschränkung > Werkzeug]* können Sie die Parameterwerte festlegen.

![!Abbildung Einstellungsbildschirm für Sicherheitswerkzeugmodellierung](../../../_assets/safety_layout/tool_sphere.PNG)


|  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |** |                       **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**                       |  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**  |
| :-------: | :------------------------------------------------: | :----------: |
| TCP X,Y,Z | <p>TCP-Position im Flanschkoordinatensystem (schreibgeschützt) – in den Werkzeuginformationen festgelegt</p> |   0  |
| Shape |   <p>Form der Werkzeugmodellierung</p><p>(Off/sphere/capsule/R-plate)</p>  | Off |
| Radius |  <p>Radius</p><p>(0.0 ~ 1000.0 mm)</p>  | 0 |
| Height |  <p>Höhe der R-Platte</p><p>(0.0 ~ 1000.0 mm)</p>  | 0 |
| Width |  <p>Breite der R-Platte</p><p>(0.0 ~ 1000.0 mm)</p>  | 0 |
| X |  <p>Modellmittelpunkt in X-Richtung</p><p>(-1000.0 ~ 1000.0 mm)</p>  | 0 |
| Y |  <p>Modellmittelpunkt in Y-Richtung</p><p>(-1000.0 ~ 1000.0 mm)</p>  | 0 |
| Z |  <p>Modellmittelpunkt in Z-Richtung</p><p>(-1000.0 ~ 1000.0 mm)</p>  | 0 |





{% hint style="warning" %}
*\[Achtung]**

* Achten Sie beim Ändern von Werkzeugdaten darauf, erneut zu überprüfen, ob die in der Sicherheitswerkzeugmodellierung eingestellten Parameter korrekt sind. Die Werkzeugdatennummer und die Sicherheitswerkzeugmodellierungsnummer desselben Werkzeugs müssen übereinstimmen.
* Da die Definition der Roboterlayout-Einstellungen nur für die Roboterachsen 2 und 3 gilt, können andere Teile des Roboters diese Zone verletzen, selbst wenn eine Sicherheitszone festgelegt ist.
{% endhint %}
