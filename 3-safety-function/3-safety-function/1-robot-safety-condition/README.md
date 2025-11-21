# 3.3.1 Roboterüberwachungsfunktion

Die Sicherheitsparameter des Roboters bestehen aus Schwellenwerten und Stoppmethoden zur Überwachung der Sicherheitsfunktionen.

Jede Sicherheitsfunktion kann verschiedene Sätze mit Aktivierungsbedingungen, Stoppmethoden bei Verstößen und Schwellenwerten speichern und verwenden.

Rufen Sie das Menü zum Einstellen der Sicherheitsparameter wie folgt auf:

* *\[시스템]**\[System]-Taste > \[4: Anwendungsparameter > 18: SafeSpace2.0 > Parametereinstellung > Roboterbeschränkung]***\[4: 응용 파라미터 > 18: SafeSpace2.0 > Parameter setup > Robot restriction]**
***


Im Menü „Roboterbeschränkung” können folgende Sicherheitsfunktionen eingestellt werden:

* **Gelenkposition: Beschränkt den Roboter so, dass er nur innerhalb eines bestimmten Bereichs pro Achse arbeiten kann.**: 로봇이 축별로 특정 범위 내에서만 동작할 수 있도록 범위를 제한
* **Gelenkgeschwindigkeit: Begrenzt das Momentum des Roboters, indem verhindert wird, dass er über einer bestimmten Geschwindigkeit pro Achse arbeitet.**: 축별 제한된 속도 이상으로 구동하지 못하게 하여 로봇의 운동량을 제한
* **Gelenkstopp-Überwachung: Überwacht den Stoppzustand des Roboters, indem nach dem Ausführen von „Stopp 2” auf abnormale Bewegungen pro Achse geprüft wird.**: 정지2 수행 후 축별로 비정상적인 움직임을 확인하여 로봇의 정지 상태를 감시
* **TCP-Geschwindigkeit: Beschränkt den Roboter so, dass er nicht über einer bestimmten Geschwindigkeit basierend auf TCP betrieben werden kann**: TCP 기준에서 로봇이 제한된 속도 이상으로 구동하지 못하게 제한
* **Re plan**: 외부 입력에 따라 로봇의 속도를 조절하여 협동 운전 모드 중 [3.2.2 Geschwindigkeits- und Abstandüberwachung](../../2-collaborative-operation-mode/2-speed-separation-monitoring.md) 수행
* **Leistung, Kollisionserkennung: Begrenzt Kraft und Druck im Falle einer Kollision zwischen Roboter und Arbeiter**: 로봇과 작업자의 충돌 발생 시의 힘과 압력을 제한
* **Momentum: Begrenzt Energie und Aufprallbelastung im Falle einer Kollision zwischen Roboter und Arbeiter**: 로봇과 작업자의 충돌 발생 시의 에너지와 충격 하중을 제한


{% hint style="warning" %}
*\[Achtung]*: Arbeiter und Anwender müssen vor der Konfiguration der Robotersicherheitsfunktionen eine Risikobewertung durchführen, um die Sicherheit von Personal und Ausrüstung in der Umgebung des Roboters zu gewährleisten, und entsprechend den Bewertungsergebnissen Folgendes festlegen:

* Unbefugte Änderungen an der Sicherheitskonfiguration durch Festlegen von Passwörtern usw. verhindern
* Sicherheitsrelevante Funktions- und Schnittstelleneinstellungen
* Vor dem Betrieb des Roboters die Richtigkeit der Einstellungen überprüfen
* Die Konformität mit der Risikobewertung für die Konfiguration und Einstellungen aller Sicherheitsfunktionen überprüfen
{% endhint %}

