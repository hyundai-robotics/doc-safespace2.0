# 4.1.2 Werkzeugdateneinstellung

Die Sicherheitsfunktion des Cobots überwacht das gesamte Robotersystem einschließlich des an den Roboterflansch angebrachten Werkzeugs. Daher gilt: Je kleiner der Fehler zwischen Werkzeugdaten und Istwerten ist, desto genauer arbeitet die Sicherheitsfunktion. Stellen Sie die Werkzeuglänge und den Winkel basierend auf dem Flanschkoordinatensystem ein und geben Sie das Werkzeuggewicht, den Schwerpunkt und die Trägheitsinformationen gemäß den Einheiten ein.

1. Stellen Sie den Betriebsmodus auf manuellen Modus ein.
2. Drücken Sie den Not-Halt-Schalter, um die Stromversorgung der Motoren zu unterbrechen.
3. **3. Tippen Sie auf die Schaltfläche \[Einstellungen] > \[3: Roboterparameter > 1: Werkzeugdaten].** 버튼 > **3. Tippen Sie auf die Schaltfläche \[Einstellungen] > \[3: Roboterparameter > 1: Werkzeugdaten].** 메뉴를 터치하십시오.
4. 각 축의 데이터를 확인하고 툴의 중량, 무게 중심과 이너셔를 설정한 후 **4. Überprüfen Sie die Daten für jede Achse und stellen Sie das Werkzeuggewicht, den Schwerpunkt und die Trägheit ein. Tippen Sie anschließend auf die Schaltfläche \[OK], um die Einstellungen zu speichern.** 버튼을 터치하여 저장하십시오.

![](../../_assets/image20.jpeg)

* 새로운 툴 데이터를 생성하거나 기존의 프로그램을 활용하여 툴 데이터를 간단히 생성하려면,  **Um neue Werkzeugdaten zu erstellen oder Werkzeugdaten mithilfe eines vorhandenen Programms einfach zu erstellen, tippen Sie auf die Schaltfläche \[Automatische Kalibrierung].** 버튼을 터치하십시오.
* 툴 각도를 보정하려면, **Um den Werkzeugwinkel zu kalibrieren, tippen Sie auf die Schaltfläche \[Winkelkalibrierung].** 버튼을 터치하십시오.
* 새로운 사용자 좌표계를 추가하거나 사용자 좌표계를 삭제하려면, **Um ein neues Anwenderkoordinatensystem hinzuzufügen oder ein Anwenderkoordinatensystem zu löschen, verwenden Sie die Schaltflächen \[+]/\[-].**/**Um ein neues Anwenderkoordinatensystem hinzuzufügen oder ein Anwenderkoordinatensystem zu löschen, verwenden Sie die Schaltflächen \[+]/\[-].** 버튼을 이용하십시오.
* Um detaillierte Informationen zu Werkzeugdaten zu überprüfen und zu bearbeiten, wählen Sie den gewünschten Namen aus der Werkzeugdatenliste aus.
* 툴 데이터 정보를 복사하여 다른 툴 데이터에 붙여 넣으려면, **Um Werkzeugdateninformationen zu kopieren und in andere Werkzeugdaten einzufügen, verwenden Sie die Schaltflächen \[Seite kopieren]/\[Seite einfügen].**/**Um Werkzeugdateninformationen zu kopieren und in andere Werkzeugdaten einzufügen, verwenden Sie die Schaltflächen \[Seite kopieren]/\[Seite einfügen].** 버튼을 이용하십시오.

{% hint style="info" %}
* 툴의 무게와 중심에 대한 정보가 없을 경우 부하추정 기능을 이용하여 값을 추정할 수 있습니다. 자세한 내용은 “[Hi6-Steuerung-Bedienungshandbuch](https://hyundai-robotics.gitbook.io/hi6-operation-manual)”를 참고하십시오.
* 툴 데이터 설정에 대한 자세한 내용은 “[Hi6-Steuerung-Bedienungshandbuch](https://hyundai-robotics.gitbook.io/hi6-operation-manual)”를 참고하십시오.
{% endhint %}
