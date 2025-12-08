# 3.1 Terminologie

### <mark style="color:green;">Roboterüberwachungsfunktion</mark>&#xD;

Parameter, die als Referenz für die Überwachung der Geschwindigkeit, Kraft und des Momentums des Roboters dienen.

* **Gelenkwinkelüberwachung**

Überwacht die Position jedes Achsengelenks. Führt einen vom Anwender festgelegten Sicherheitshalt durch, wenn der Referenzwert überschritten wird.

* **Gelenkgeschwindigkeitsüberwachung**

Überwacht die Geschwindigkeit jedes Achsengelenks. Führt einen vom Anwender festgelegten Sicherheitshalt durch, wenn der Referenzwert überschritten wird.
    
* **Überwachung des sicheren Betriebshalts (SOS, Safe Operating Stop)**

Überwacht, ob jede Achse ohne Schlupf im Stillstand bleibt. Führt einen Stopp der Kategorie 0 aus, wenn der Referenzwert überschritten wird.

* **TCP-Positionsüberwachung**

Überwacht, ob das Sicherheitswerkzeugmodell die Sicherheitszone verletzt. Führt einen vom Anwender festgelegten Sicherheitshalt aus, wenn die Zone verletzt wird.
    
* **TCP-Orientierungsüberwachung**

Überwacht, ob die Werkzeugausrichtung innerhalb des festgelegten Bereichs bleibt. Führt einen vom Anwender festgelegten Sicherheitshalt durch, wenn der Referenzwert überschritten wird.
    
* **TCP-Geschwindigkeitsüberwachung**

Überwacht die Geschwindigkeit der Werkzeugspitze. Führt einen vom Anwender festgelegten Sicherheitshalt durch, wenn der Referenzwert überschritten wird.
    
* **Leistungsüberwachung**

Überwacht die Leistung des Roboters. Führt einen vom Anwender festgelegten Sicherheitshalt durch, wenn der Referenzwert überschritten wird.
    
* **Momentenüberwachung**

Überwacht das Moment des Roboters. Führt einen vom Anwender festgelegten Sicherheitshalt durch, wenn der Referenzwert überschritten wird.


* **Kollisionserkennung**

Führt einen vom Anwender festgelegten Sicherheitshalt durch, wenn eine auf den Roboter ausgeübte externe Kraft den zulässigen Wert überschreitet.


### <mark style="color:green;">Sicherheitslayout</mark>

Parameter für Sicherheitszonen und Werkzeugzonen, die als Referenzen für die Überwachung der TCP-Position und -Orientierung dienen.

* **Sicherheitszone**

Allgemeiner Begriff für den Arbeitsbereich und den geschützten Bereich des Werkzeugs.
* **Arbeitsbereich**

Der Bereich, in dem der Roboter seine Arbeit verrichtet. Führt einen Sicherheitshalt durch, wenn das Werkzeug und das Roboter-Ellbogenmodell den Arbeitsbereich verlassen.
* **Geschützter Bereich**

Der Bereich, der vor dem Roboter geschützt werden muss. Es wird ein Sicherheitshalt ausgeführt, wenn das Werkzeug und das Roboter-Ellbogenmodell den geschützten Raum verletzen.
* **Sicherheitswerkzeugmodellierung**

Modellierung des am Roboter befestigten Werkzeugs als Kugel und Kegel zur TCP-Positions- und Orientierungsüberwachung.
* **Sicherheitsroboter-Modellierung**

Modellierung der Achsen 2 und 3 des Roboters als Kapseln zur Überwachung des Abstands zur Sicherheitszone



### <mark style="color:green;">Sicherheitsstopp</mark>&#xD;

Anhalten des Roboters, um einen sicheren Zustand zu schaffen, wenn die Sicherheit verletzt wird. Es gibt 3 Stoppmethoden. Ausführliche Informationen zu den einzelnen Stoppmethoden finden Sie in „ISO 13850” oder „IEC 60204-1”.

* **Stopp 0**

Sofortige Unterbrechung der Stromversorgung aller Gelenkmotoren und Stopp (unkontrollierter Stopp)
* **Stopp 1**

Die Motoren aller Gelenke werden abgebremst und gestoppt, anschließend wird die Stromversorgung der Motoren unterbrochen (kontrollierter Stopp). Der Roboter folgt während der Abbremsung weiterhin dem Programmweg und die Stromversorgung wird unterbrochen, sobald der Roboter zum Stillstand kommt.
* **Stopp 2**

Die Motoren aller Gelenke werden abgebremst, und anschließend wird die Überwachung des sicheren Betriebshalts (SOS) aktiviert. Die Stromversorgung aller Motoren wird aufrechterhalten.


Stopp 1 und Stopp 2 überwachen den Verzögerungsvorgang anhand der Verzögerungszeit und -strecke.

* **Stoppzeit**

Überwacht die Zeit vom Beginn der Verzögerung bis zum tatsächlichen Stillstand. Wenn der Roboter nicht innerhalb der festgelegten Zeit zum Stillstand kommt, wird Stopp 0 ausgeführt, um die Stromversorgung der Motoren sofort zu unterbrechen.
* **Stoppweg**

Überwacht den TCP-Weg vom Beginn der Verzögerung bis zum tatsächlichen Stillstand. Wenn der Roboter nicht innerhalb des festgelegten Weges zum Stillstand kommt, wird „Stopp 0” ausgeführt, um die Motoren sofort vom Stromnetz zu trennen.



### <mark style="color:green;">Sichere Bewegungsoptimierung</mark>&#xD;

Diese Funktion passt die Roboterbewegung automatisch an, um ein Überschreiten der eingegebenen Parameter zu vermeiden.
Folgende Parameter werden bei der Bewegungsoptimierung berücksichtigt:

* **Gelenkgeschwindigkeit**

* **TCP-Geschwindigkeit**

* **Leistung**

* **Impuls**

* **Stoppzeit**

* **Stoppweg**