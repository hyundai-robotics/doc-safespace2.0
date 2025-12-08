# 3.3.1.5 Wartung

Im Wartungsmenü können Sie die Prüfzyklen für die Referenzfahrt und die Bremsen einstellen. Die regelmäßige Überwachung des Ausgangs- und Bremsstatus jeder Roboterachse ist unerlässlich, um die Funktionsfähigkeit der Sicherheitsfunktionen zu gewährleisten. Sollten die Tests innerhalb des eingestellten Zyklus nicht abgeschlossen werden, wird Sicherheitsstopp 1 sofort aktiviert.

Um einen Bremsentest durchzuführen,

können Sie die Parameterwerte im Menü **\[System > 8: Sicherheitssystem > 1: Grundeinstellungen > 5: Wartung]** einstellen.

<p align="center">
<img src="../../../_assets/3/maint_param.png"></img>
<em><p align="center">유지 보수 설정 화면</p></em>
</p>


|  **Parameter** |                       **Beschreibung**                       |  **Standardwert**  |
| :-------: | :------------------------------------------------: | :-------------: |
| <p>Mastering-Ausführungszyklus</p><p>[h]</p> | <p>Mastering-Testausführungszyklus</p><p>(2 ~ 720)</p> | 720 |
| <p>Unterbrechung des Testausführungszyklus</p><p>[h]</p> | <p>Unterbrechung des Testausführungszyklus</p><p>(2 ~ 720)</p> | 720 |


{% hint style="warning" %}
**\[Vorsicht]**: Im Falle eines Absturzes empfehlen wir die Durchführung eines Mastering-Tests und eines Break-Tests.  
{% endhint %}
 