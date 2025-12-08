# 1.3 Risikobewertung

In der integrierten Systemkonfiguration einschließlich des Roboters ist die Risikobewertung einer der wichtigen Faktoren, die in den meisten Ländern als gesetzliche Anforderung behandelt wird. Da die Sicherheitsbewertung einer Roboterinstallation davon abhängt, wie der Roboter in das System integriert ist, kann das Risiko des integrierten Systems nicht allein anhand des Roboters bewertet werden.

Der Systemadministrator muss das System gemäß den Richtlinien von ISO 12100 und ISO 10218-2 konfigurieren und betreiben, um eine Risikobewertung durchzuführen. Sie können auch die technische Spezifikation ISO/TS 15066 zu Rate ziehen.

Bei der Risikobewertung muss der gesamte Prozess des integrierten Systems einschließlich des Roboters berücksichtigt werden. Die Hauptziele der Risikobewertung sind wie folgt:

* Grundeinstellungen für den Einsatz und das Teachen des Roboters
* Fehlerdiagnose und Wartung
* Normaler Betrieb des installierten Roboters

Nach der Installation des Roboters und der Konfiguration des Systems muss eine Risikobewertung durchgeführt werden. Die Risikobewertung dient in erster Linie dazu, die Eignung der Sicherheitsvorrichtungen im Roboterintegrationssystem zu bestimmen, einschließlich der Notwendigkeit zusätzlicher Not-Halt- und anderer Sicherheitsvorrichtungen.

Es ist sehr wichtig, geeignete Sicherheitsvorrichtungen zu identifizieren und das roboterintegrierte System korrekt zu konfigurieren. Konfigurieren Sie das integrierte System unter Bezugnahme auf die entsprechenden Inhalte im Handbuch.

Sie können Grenzwerte für die TCP-Geschwindigkeit, den Druck, die Leistung, das Moment, die Kollisionserkennung, das Untersetzungsverhältnis, den Gelenkwinkel pro Achse, die Geschwindigkeit usw. des Roboters festlegen. Sie können auch Sicherheitsfunktionen mithilfe von sicherheitsrelevanten E/A und Kommunikation konfigurieren. Ausführliche Informationen zur Konfiguration der Sicherheitsfunktionen finden Sie unter "[**3. SafeSpace2.0-Sicherheitsfunktionen](../3-safety-function/README.md)".

**\[Sicherheitsfunktion]** Im Menü können Sie sicherheitsrelevante Funktionen konfigurieren. Die folgenden Funktionen stehen zur Verfügung:

* **Kraft- und Leistungsbegrenzung**: Begrenzt die Kraft und den Druck zum Anhalten, um eine Kollision zwischen dem Roboter und dem Arbeiter zu verhindern
* **Momentbegrenzung**: Reduziert die Betriebsgeschwindigkeit des Roboters, um die Energie und die Stoßbelastung zu begrenzen und eine Kollision zwischen dem Roboter und dem Arbeiter zu verhindern
* **Gelenk- und TCP-Positionsbegrenzung**: Beschränkt die Bewegung, um zu verhindern, dass sich der Roboter zu bestimmten Körperteilen wie dem Hals oder Kopf des Anwenders bewegt
* **TCP- und Werkzeuglagenbegrenzung**: Beschränkt die Bewegung, um Risiken im Zusammenhang mit bestimmten Bereichen oder Merkmalen des Werkzeugs und des Werkstücks zu reduzieren (z. B. um zu verhindern, dass sich scharfe Teile des Werkzeugs oder Werkstücks auf den Arbeiter zubewegen)
* **Geschwindigkeitsbegrenzung**: Begrenzt die Bewegung des Roboters auf eine niedrige Geschwindigkeit, um dem Arbeiter Zeit zu geben, eine Kollision zu vermeiden, falls es zu einer Kollision zwischen dem Roboter und dem Arbeiter kommen sollte

Darüber hinaus können Sie sicherheitsrelevante Funktionen konfigurieren, indem Sie den Roboter an einem bestimmten Ort installieren oder Sicherheits-E/A verwenden.

Wichtige Punkte bei der Risikobewertung des Roboterintegrationssystems sind:

* Schweregrad der Kollision durch den Roboter
* Wahrscheinlichkeit einer Kollision durch den Roboter
* Möglichkeit der Kollisionsvermeidung durch den Roboter

Wenn bei der Konfiguration des integrierten Systems die Risikofaktoren durch die sicherheitsrelevanten Funktionen des Roboters nicht ausreichend beseitigt werden können (z. B. Verwendung von Werkzeugen für nicht kollaborative Roboter usw.), müssen Sie durch eine Risikobewertung die erforderlichen zusätzlichen Schutzvorrichtungen installieren.
