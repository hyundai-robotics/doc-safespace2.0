# 4.1.1 Encoder-Prüfung

Da die Sicherheitsfunktion die Position und Geschwindigkeit des Roboters anhand der Encoder-Daten jeder Achse diagnostiziert, ist die Genauigkeit der Encoder-Daten von großer Bedeutung. Daher müssen Sie vor der Verwendung der Sicherheitsfunktion überprüfen, ob die Encoderwerte mit den tatsächlichen Werten übereinstimmen.

1\. Überprüfen Sie die Nullpunktmarkierung jeder Roboterachse und verfahren Sie die Achse.


Sollte es aufgrund einer Verletzung der Sicherheitsfunktion zu einem Stopp kommen, verfahren Sie jede Achse im Handbetrieb mit Hilfe der Jog-Funktion. Detaillierte Informationen zu Wiederherstellungsmethoden finden Sie unter "[**6.1 Wiederherstellungsmodus**](../../6-recovery/README.md)".

2\. Überprüfen Sie im Pose-Informationsfenster im Arbeitsbereich, ob die Achskoordinatenwerte des Roboters als Referenzhaltung (**0, 90, 0, 0, 0, 0** \[deg]) angezeigt werden.


* Wenn im Arbeitsbereich kein Pose-Informationsfenster vorhanden ist, tippen Sie auf die Schaltfläche **\[+]** oben rechts im Bedienfeldstapel und anschließend im Bedienfeldauswahlfenster auf **\[Pose]**.


3\. Wenn der Winkelwertfehler innerhalb von 0,01 liegt, fahren Sie mit dem nächsten Schritt fort. Wenn der Fehler 0,01 überschreitet, führen Sie den Encoder-Offset durch.

4\. Starten Sie das System neu.

{% hint style="info" %}
Weitere Informationen zum Encoder-Offset finden Sie unter „[**7.4.4 Encoder-Offset**](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/korean-tp630/README)“ im „[**Hi6 Controller Operating Manual**](https://hrbook.hrc.web.app/#/view/doc-hi6-operation/korean-tp630/7-system/4-robot-parameter/4-encoder-offset/README)“.
{% endhint %}
