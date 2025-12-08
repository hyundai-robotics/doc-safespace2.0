# 3.3.2 Roboterüberwachungsfunktion

Die Sicherheitsparameter des Roboters umfassen Grenzwerte und Abschaltmethoden zur Überwachung der Sicherheitsfunktionen.

Jede Sicherheitsfunktion kann mit verschiedenen Aktivierungsbedingungen, Abschaltmethoden bei Überschreitung und Grenzwerten konfiguriert werden.

Um die Sicherheitsparameter des Roboters zu konfigurieren, rufen Sie das Menü wie folgt auf:

* **\[System > 8: Sicherheitssystem > 2: Parametereinstellungen > 1: Robotergrenzen]**
****

Folgende Sicherheitsfunktionen können im Menü „Robotergrenzen“ konfiguriert werden:

* **Gelenkbereich**: Begrenzt den Bewegungsbereich des Roboters für jede Achse auf einen bestimmten Wert.
* **Gelenkgeschwindigkeit**: Begrenzt die Bewegung des Roboters, indem die Geschwindigkeitsbegrenzung für jede Achse nicht überschritten wird.
* **Gelenkstopp**: Überwacht den Stillstand des Roboters, indem nach dem zweiten Stopp jede Achse auf ungewöhnliche Bewegungen überprüft wird.
* **TCP-Geschwindigkeit**: Begrenzt die Geschwindigkeit des Roboters auf einen festgelegten Wert gemäß TCP-Standard.
* **Kollisionserkennung**: Begrenzt die Kraft bei einer Kollision zwischen Roboter und Arbeiter.
* **RePlan**: Passt die Robotergeschwindigkeit gemäß externer Eingaben an, um im kollaborativen Betriebsmodus die Geschwindigkeits- und Positionsüberwachung (siehe [3.2.2 Geschwindigkeits- und Positionsüberwachung](../../2-collaborative-operation-mode/2-speed-separation-monitoring.md)) durchzuführen.
* **Krafterkennung**: Begrenzt die Kraft bei einer Kollision zwischen Roboter und Arbeiter.
* **Impuls**: Begrenzt die Energie und die Aufprallbelastung bei einer Kollision zwischen Roboter und Arbeiter.


{% hint style="warning" %}
**\[Achtung]**: Bediener und Benutzer müssen vor der Konfiguration der Sicherheitsfunktionen des Roboters eine Risikobewertung durchführen, um die Sicherheit von Personal und Ausrüstung im Umfeld des Roboters zu gewährleisten. Konfigurieren Sie basierend auf den Ergebnissen der Bewertung Folgendes:

* Legen Sie ein Passwort fest, um unbefugte Änderungen an der Sicherheitskonfiguration zu verhindern.
* Konfigurieren Sie sicherheitsrelevante Funktionen und Schnittstellen.
* Überprüfen Sie die Richtigkeit der Einstellungen, bevor Sie den Roboter in Betrieb nehmen.
* Stellen Sie sicher, dass alle Konfigurationen und Einstellungen der Sicherheitsfunktionen der Risikobewertung entsprechen.
{% endhint %}

