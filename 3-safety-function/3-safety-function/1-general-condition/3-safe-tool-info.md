# 3.3.1.3 Sicherheitswerkzeuginformationen

Die Sicherheitswerkzeuginformationen werden von der Sicherheitssteuerung zur Berechnung von Geschwindigkeit und Position des Roboters verwendet. Sie müssen die Werkzeuginformationen des jeweiligen Roboters eingeben. Diese müssen mit der Werkzeugnummer für die Robotersteuerung übereinstimmen (**\[System > 3: Roboterparameter > 1: Werkzeugdaten]**).


Sie können Sicherheitswerkzeuginformationen im Menü **\[System > 8: Sicherheitssystem > 1: Grundeinstellungen > 3: Sicherheitswerkzeuginformationen]** festlegen und Werkzeuginformationen, die für die Robotersteuerung verwendet werden, laden, indem Sie unten im Menü auf „Werkzeugdaten laden“ klicken.

<p align="center">
<img src="../../../_assets/3/tool_info_param.png"></img>
<em><p align="center">안전 툴 정보 설정 화면</p></em>
</p>


|  **Parameter** |                       **Beschreibung**                       |  **Standardwert**  |
| :-------: | :------------------------------------------------: | :-------------: |
| <p>Gewicht</p><p>[kg]</p> | <p>Gewicht des Werkzeugs</p><p>(0,0 ~ 1000,0)</p> | 0,0 |
| <p>Länge</p><p>[mm]</p> | <p>Länge des Werkzeugs</p><p>(-3000,0 ~ 3000,0)</p> | 0,0 |
| <p>Mitte</p><p>[mm]</p> | <p>Position des Werkzeugschwerpunkts relativ zur Flanschmitte</p><p>(-3000,0 ~ 3000,0)</p> | 0,0 |
| <p>Trägheit</p><p>[···]</p> | <p>Trägheitsmoment des Werkzeugs bezüglich der Werkzeugkoordinaten</p><p>(0,0 ~ 2000,000)</p> | 0,0 |
| Werkzeugdaten laden | Funktion zum Laden von Werkzeuginformationen für die Robotersteuerung anhand der Werkzeugnummer | - |
| Kopieren | Funktion zum Kopieren der auf der entsprechenden Seite eingegebenen Werte | - |
| Einfügen | Funktion zum Einfügen der Werte der kopierten Seite auf die entsprechende Seite | - |

{% hint style="warning" %}
**\[Achtung]**: Stimmen die Informationen zum Sicherheitswerkzeug nicht mit den für die Robotersteuerung verwendeten Werkzeuginformationen überein, wird eine Warnung/Fehlermeldung ausgegeben und der Roboter kann nicht betrieben werden. Stellen Sie sicher, dass die tatsächlichen Werkzeuginformationen mit den Informationen zum Sicherheitswerkzeug übereinstimmen, bevor Sie den Roboter in Betrieb nehmen.
{% endhint %}
 
{% hint style="warning" %}
**\[Achtung]**: Es werden nur die Sicherheitswerkzeugnummern 0 bis 15 unterstützt. Wenn Ihr System Werkzeuginformationen 16 bis 31 verwendet, ordnen Sie die Sicherheitswerkzeugnummer 0 den entsprechenden Werkzeuginformationen zu.
{% endhint %}
 