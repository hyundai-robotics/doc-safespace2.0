# 3.3.2.4 TCP-Orientierungsüberwachung

Um die TCP-Orientierungsüberwachungsfunktion zu verwenden, können Sie einen Überwachungskegel einrichten, indem Sie den Drehwinkel und den Abweichungswinkel für die Erzeugung des Referenzvektors festlegen.

Durch Festlegen des Referenzvektors (![](../../../_assets/3.png)) mittels Drehung des Z-Richtungsvektors des Roboterkoordinatensystems (![](../../../_assets/1.png)) um einen festgelegten Winkel lässt sich ein Kegel (![](../../../_assets/2.png)) modellieren, der aus durch den Abweichungswinkel (![](../../../_assets/4.png)) getrennten Mutterlinien besteht. Die Spitze dieses Kegels (![](../../../_assets/5.png)) befindet sich am TCP. Überschreitet der Z-Richtungsvektor des TCP (![](../../../_assets/6.png)) den Überwachungskegel, tritt ein Fehler aufgrund einer Verletzung der TCP-Richtungsgrenzfunktion auf.

<p align="center">
<img src="../../../_assets/safety_layout/tool_ori.png"></img>
<em><p align="center">툴 방향 제한 기능</p></em>
</p>

Die Parameterwerte können Sie im Menü **\[System > 8: Sicherheitssystem > 2: Parametereinstellung > 2: Bereichsbegrenzung > 4: Werkzeugrichtung]** einstellen.

<p align="center">
<img src="../../../_assets/safety_layout/tool_orient.png"></img>
<em><p align="center">툴 방향 설정 화면</p></em>
</p>

|  **Parameter** |                       **Beschreibung**                       |  **Standardeinstellung**  |
| :-------: | :------------------------------------------------: | :----------: |
| Aktivierung | <p>Funktionsstatus</p><p>(Ungültig / Gültig / Sichere E/A)</p> | Ungültig |
| Stoppmethode | <p>Stoppmethode bei Funktionsverletzung</p><p>(Stop 0 / Stop 1 / Stop 2 / Kein Stopp)</p> | Stop 1 |
| <p>Org.Rx</p><p>[deg]</p> | <p>Drehwinkel des Referenzvektors relativ zur X-Richtung</p><p>(-180,0 ~ 180,0)</p> | 0,0 |
| <p>Org.Ry</p><p>[deg]</p> | <p>Drehwinkel des Referenzvektors relativ zur Y-Richtung</p><p>(-180,0 ~ 180,0)</p> | 0,0 |
| <p>Org.Rz</p><p>[deg]</p> | <p>Rotation des Referenzvektors relativ zur Z-Richtung</p><p>(-180,0 ~ 180,0)</p> | 0,0 |
| Abweichungswinkel | <p>Werkzeugorientierungsgrenze</p><p>(-180,0 ~ 180,0)</p> | 0,0 |
| Aktuelle Position laden <br> | Referenzvektor mit aktueller Roboterposition erstellen | - |


{% hint style="warning" %}
**\[Achtung]**

* Achten Sie beim Ändern von Werkzeugdaten darauf, erneut zu überprüfen, ob die in der Sicherheitswerkzeugmodellierung eingestellten Parameter korrekt sind. Die Werkzeugdatennummer und die Sicherheitswerkzeugmodellierungsnummer desselben Werkzeugs müssen übereinstimmen.
{% endhint %}
