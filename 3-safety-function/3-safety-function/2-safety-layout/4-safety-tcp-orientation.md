# 3.3.2.4 TCP-Orientierungsüberwachung

Um die TCP-Orientierungsüberwachungsfunktion zu verwenden, können Sie einen Überwachungskegel einrichten, indem Sie den Drehwinkel und den Abweichungswinkel für die Erzeugung des Referenzvektors festlegen.

Der Z-Richtungsvektor des Roboterkoordinatensystems (!\) wird um den eingestellten Winkel gedreht, um den Referenzvektor (!\) festzulegen, und ein Kegel (!\) bestehend aus Generatricen mit einem Abweichungswinkel (!\) davon kann modelliert werden. Der Scheitelpunkt (!\) eines solchen Kegels befindet sich am TCP, und ein Verstoß gegen die TCP- Orientierungseinschränkungsfunktion tritt auf, wenn der TCP-Z-Richtungsvektor (!\) den Überwachungskegel überschreitet.

![!Abbildung TCP-Orientierungseinschränkungsfunktion](../../../_assets/safety_layout/tool_ori.png)

Über das Menü \[System > 4: Anwendungsparameter > 18: SafeSpace2.0 > Parametereinstellungen > Layoutbeschränkung > TCP-Orientierung]* können Sie die Parameterwerte festlegen.

![!Abbildung Bildschirm „TCP-Orientierungseinstellung”](../../../_assets/safety_layout/tool_ori_param.PNG)


|  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |** |                       **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**                       |  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Funktionsaktivierungsstatus</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stoppmethode bei Funktionsverletzung</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Rx |   <p>Drehwinkel des Referenzvektors basierend auf der X-Richtung</p><p>(-180.0 ~ 180.0 (deg))</p>  |  0.0 |
| Ry |   <p>Drehwinkel des Referenzvektors basierend auf der Y-Richtung</p><p>(-180.0 ~ 180.0 (deg))</p>  |  0.0 |
| Rz |   <p>Drehwinkel des Referenzvektors basierend auf der Z-Richtung</p><p>(-180.0 ~ 180.0 (deg))</p>  |  0.0 |
| Abweichungswinkel |   <p>TCP-Orientierungsgrenzwert</p><p>(-180.0 ~ 180.0 (deg))</p>  |  0.0 |





{% hint style="warning" %}
*\[Achtung]**

* Achten Sie beim Ändern von Werkzeugdaten darauf, erneut zu überprüfen, ob die in der Sicherheitswerkzeugmodellierung eingestellten Parameter korrekt sind. Die Werkzeugdatennummer und die Sicherheitswerkzeugmodellierungsnummer desselben Werkzeugs müssen übereinstimmen.
{% endhint %}
