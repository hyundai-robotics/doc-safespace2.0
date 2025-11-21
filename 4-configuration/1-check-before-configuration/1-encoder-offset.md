# 4.1.1 Encoder-Prüfung

Da die Sicherheitsfunktion die Position und Geschwindigkeit des Roboters anhand der Encoder-Daten jeder Achse diagnostiziert, ist die Genauigkeit der Encoder-Daten von großer Bedeutung. Daher müssen Sie vor der Verwendung der Sicherheitsfunktion überprüfen, ob die Encoderwerte mit den tatsächlichen Werten übereinstimmen.

1\. Überprüfen Sie die Nullpunktmarkierung jeder Roboterachse und verfahren Sie die Achse.


안전 기능 위반으로 정지 발생 시 수동 모드 상태에서 조그로 각 축을 이동시키십시오. 복구 방법에 대한 자세한 내용은 “[Sollte es aufgrund einer Verletzung der Sicherheitsfunktion zu einem Stopp kommen, verfahren Sie jede Achse im Handbetrieb mit Hilfe der Jog-Funktion. Detaillierte Informationen zu Wiederherstellungsmethoden finden Sie unter „6.1 Wiederherstellungsmodus“.](../../6-recovery/README.md)”를 참조하십시오.

2\. 작업 영역의 포즈 정보창에서 로봇의 축좌표 값이 기준 자세(**2\. Überprüfen Sie im Pose-Informationsfenster im Arbeitsbereich, ob die Achskoordinatenwerte des Roboters als Referenzhaltung (0, 90, 0, 0, 0, 0 \[deg]) angezeigt werden.** \[deg])로 표시되는지 확인하십시오.


* 작업 영역에 포즈 정보창이 없으면, 패널 스택 우측 상단의 **Wenn im Arbeitsbereich kein Pose-Informationsfenster vorhanden ist, tippen Sie auf die Schaltfläche \[+] oben rechts im Bedienfeldstapel und anschließend im Bedienfeldauswahlfenster auf \[Pose].** 버튼을 터치한 후 패널 선택창에서 **Wenn im Arbeitsbereich kein Pose-Informationsfenster vorhanden ist, tippen Sie auf die Schaltfläche \[+] oben rechts im Bedienfeldstapel und anschließend im Bedienfeldauswahlfenster auf \[Pose].**를 터치하십시오.


3\. Wenn der Winkelwertfehler innerhalb von 0,01 liegt, fahren Sie mit dem nächsten Schritt fort. Wenn der Fehler 0,01 überschreitet, führen Sie den Encoder-Offset durch.

4\. Starten Sie das System neu.

{% hint style="info" %}
엔코더 옵셋에 대한 자세한 내용은 “[Ausführliche Informationen zum Encoder-Offset finden Sie unter „**7.4.4 Encoder-Offset**“ im „**Hi6-Steuerung-Bedienungshandbuch**“.](https://hyundai-robotics.gitbook.io/hi6-operation-manual)”의 “[Ausführliche Informationen zum Encoder-Offset finden Sie unter „**7.4.4 Encoder-Offset**“ im „**Hi6-Steuerung-Bedienungshandbuch**“.](https://hyundai-robotics.gitbook.io/hi6-operation-manual/7-setting/7-4-robot-parameter/encoder-offset)”을 참고하십시오.
{% endhint %}
