# 3.3.1.4 Sicherheitszusatzgewicht

Die Sicherheitszusatzgewichtsinformationen werden von der Sicherheitssteuerung zur Berechnung des Drehmoments des Roboters verwendet. Sie müssen die Informationen zum tatsächlich am Roboter installierten Zusatzgewicht eingeben. Diese Informationen müssen mit den für die Robotersteuerung verwendeten Zusatzgewichtsinformationen übereinstimmen (**\[System > 3: Roboterparameter > 7: Zusatzgewicht nach Achse]**).


* **\[System > 8: Sicherheitssystem > 1: Grundeinstellungen > 4: Sicherheitszusatzgewicht]** Sie können die Sicherheitszusatzgewichtsinformationen im Menü einstellen und die für die Robotersteuerung verwendeten Zusatzgewichtsinformationen laden, indem Sie unten im Menü auf „Zusatzgewicht laden“ klicken.


<p align="center">
<img src="../../../_assets/3/add_tool_param.png"></img>
<em><p align="center">안전 부가중량 설정 화면</p></em>
</p>


|  **Parameter** |                       **Beschreibung**                       |  **Standardwert**  |
| :-------: | :------------------------------------------------: | :-------------: |
| <p>Gewicht</p><p>[kg]</p> | <p>Gewicht des Werkzeugs</p><p>(0,0 ~ 1000,0)</p> | 0,0 |
| <p>Zentrum</p><p>[mm]</p> | <p>Position des Werkzeugschwerpunkts relativ zur Flanschmitte</p><p>(-3000,0 ~ 3000,0)</p> | 0,0 |
| <p>Trägheitsmoment</p><p>[m·m]</p> | <p>Trägheitsmoment des Werkzeugs bezüglich der Werkzeugkoordinaten</p><p>(0,0 ~ 2000,000)</p> | 0,0 |
| Zusätzliches Gewicht laden | Eine Funktion zum Laden zusätzlicher Gewichtsinformationen für die Robotersteuerung | - |
| Kopieren | Eine Funktion zum Kopieren der auf der entsprechenden Seite eingegebenen Werte | - |
| Einfügen | Eine Funktion zum Einfügen der Werte von der kopierten Seite auf die entsprechende Seite | - |

{% hint style="warning" %}
**\[Achtung]**: Stimmen die Sicherheitsgewichtsangaben und die für die Robotersteuerung verwendeten Gewichtsangaben nicht überein, wird eine Warnung/Fehlermeldung ausgegeben und der Roboter kann nicht betrieben werden. Stellen Sie sicher, dass die Gewichtsangaben mit dem tatsächlichen angehängten Gewicht übereinstimmen, bevor Sie den Roboter in Betrieb nehmen. 
{% endhint %}
 
{% hint style="warning" %}
**\[Achtung]**: Die Sicherheitszusatzgewichtsnummer kann zwischen 0 und 2 liegen. Jede Nummer entspricht der Achsennummer des Systemzusatzgewichts (0 – Südachse, 1 – Horizontalachse, 2 – Vertikalachse). Bitte geben Sie die Zusatzgewichtsinformationen ein, indem Sie die Sicherheitsparameternummer der Achsennummer zuordnen.
{% endhint %}
 
 