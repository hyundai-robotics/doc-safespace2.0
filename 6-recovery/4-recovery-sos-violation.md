# 6.4	Wiederherstellung nach einem Verstoß gegen den sicheren Betriebshalt (SOS)

Ein Verstoß gegen den sicheren Betriebshalt (SOS) liegt vor, wenn eine Bewegung erkannt wird, während der Robotermotor eingeschaltet ist und sich im Stillstand befindet. Im Falle eines Verstoßes gegen den sicheren Betriebshalt erkennt der Roboter eine momentane Bewegung und generiert einen Fehler, sodass der Fehler behoben werden kann, ohne die Position des Roboters zu verändern.

1. Stellen Sie den Betriebsartenschalter auf „Manuell”, um in den Handbetrieb zu wechseln.


2. Entfernen Sie externe Faktoren, die Kraft auf den Roboter ausüben.


3.  안전 상태 모니터링 화면에서 각 영역의 상태가 **3. Überprüfen Sie im Bildschirm zur Überwachung des Sicherheitsstatus, ob der Status jeder Zone als „SAFE“ angezeigt wird.**로 나타나는지 확인하십시오.


{% hint style="warning" %}
*[Achtung]**

* Bitte überprüfen Sie nach der Fehlerbehebung die Parameter für die Überwachung des sicheren Betriebshalts.
* Schalten Sie den Motor im Automatikmodus ein und überprüfen Sie, ob der Fehler erneut auftritt.
* Wenn derselbe Fehler erneut auftritt, überprüfen Sie den Motor und das Getriebe der entsprechenden Achse.
{% endhint %}
