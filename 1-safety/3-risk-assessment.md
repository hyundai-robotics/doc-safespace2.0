# 1.3 Risikobewertung

In der integrierten Systemkonfiguration einschließlich des Roboters ist die Risikobewertung einer der wichtigen Faktoren, die in den meisten Ländern als gesetzliche Anforderung behandelt wird. Da die Sicherheitsbewertung einer Roboterinstallation davon abhängt, wie der Roboter in das System integriert ist, kann das Risiko des integrierten Systems nicht allein anhand des Roboters bewertet werden.

Der Systemadministrator muss das System gemäß den Richtlinien von ISO 12100 und ISO 10218-2 konfigurieren und betreiben, um eine Risikobewertung durchzuführen. Sie können auch die technische Spezifikation ISO/TS 15066 zu Rate ziehen.

Bei der Risikobewertung muss der gesamte Prozess des integrierten Systems einschließlich des Roboters berücksichtigt werden. Die Hauptziele der Risikobewertung sind wie folgt:

* Grundeinstellungen für den Einsatz und das Teachen des Roboters
* Fehlerdiagnose und Wartung
* Normaler Betrieb des installierten Roboters

Nach der Installation des Roboters und der Konfiguration des Systems muss eine Risikobewertung durchgeführt werden. Die Risikobewertung dient in erster Linie dazu, die Eignung der Sicherheitsvorrichtungen im Roboterintegrationssystem zu bestimmen, einschließlich der Notwendigkeit zusätzlicher Not-Halt- und anderer Sicherheitsvorrichtungen.

Es ist sehr wichtig, geeignete Sicherheitsvorrichtungen zu identifizieren und das roboterintegrierte System korrekt zu konfigurieren. Konfigurieren Sie das integrierte System unter Bezugnahme auf die entsprechenden Inhalte im Handbuch.

로봇의 TCP 속도, 압력, 파워, 모멘텀, 충돌 검지, 감속비의 제한치, 조인트별 각도, 속도 등의 제한치 등을 설정할 수 있습니다. 또한, 안전 관련 I/O 및 통신을 이용하여 안전 기능을 구성할 수 있습니다. 안전 기능 구성에 대한 자세한 내용은 “[Sie können Grenzwerte für die TCP-Geschwindigkeit, den Druck, die Leistung, das Moment, die Kollisionserkennung, das Untersetzungsverhältnis, den Gelenkwinkel pro Achse, die Geschwindigkeit usw. des Roboters festlegen. Sie können auch Sicherheitsfunktionen mithilfe von sicherheitsrelevanten E/A und Kommunikation konfigurieren. Ausführliche Informationen zur Konfiguration der Sicherheitsfunktionen finden Sie unter „**3. SafeSpace2.0-Sicherheitsfunktionen“](../3-safety-function/README.md)”를 참조하십시오.

Im Menü \\[Sicherheitsfunktion]* können Sie sicherheitsrelevante Funktionen konfigurieren. Die folgenden Funktionen stehen zur Verfügung:

* **Kraft- und Leistungsbegrenzung: Begrenzt die Kraft und den Druck zum Anhalten, um eine Kollision zwischen dem Roboter und dem Arbeiter zu verhindern.**: 로봇과 작업자의 충돌을 대비하여 정지하는 힘과 압력을 제한
* **Momentbegrenzung: Reduziert die Betriebsgeschwindigkeit des Roboters, um die Energie und die Stoßbelastung zu begrenzen und eine Kollision zwischen dem Roboter und dem Arbeiter zu verhindern.**: 로봇과 작업자의 충돌을 대비하여 로봇의 동작 속도를 줄여 에너지와 충격 하중을 제한
* **Gelenk- und TCP-Positionsbegrenzung: Beschränkt die Bewegung, um zu verhindern, dass sich der Roboter zu bestimmten Körperteilen wie dem Hals oder Kopf des Anwenders bewegt**: 로봇이 사용자의 목이나 머리와 같은 특정 신체 부위로 이동하지 않도록 움직임을 제한
* **TCP- und Werkzeuglagenbegrenzung: Beschränkt die Bewegung, um Risiken im Zusammenhang mit bestimmten Bereichen oder Merkmalen des Werkzeugs und des Werkstücks zu reduzieren (z. B. um zu verhindern, dass sich scharfe Teile des Werkzeugs oder Werkstücks auf den Arbeiter zubewegen)**: 툴과 작업 부품의 특정 영역이나 특징과 관련된 위험을 줄이기 위해 움직임을 제한(예: 툴 또는 작업물의 날카로운 부분이 작업자를 향해 이동하는 것을 막기 위함)
* **Geschwindigkeitsbegrenzung: Begrenzt die Bewegung des Roboters auf eine niedrige Geschwindigkeit, um dem Arbeiter Zeit zu geben, eine Kollision zu vermeiden, falls es zu einer Kollision zwischen dem Roboter und dem Arbeiter kommen sollte.**: 로봇과 작업자의 충돌을 대비하여 작업자가 충돌을 피할 시간을 제공하기 위해 로봇의 움직임이 저속으로 유지되도록 제한

Darüber hinaus können Sie sicherheitsrelevante Funktionen konfigurieren, indem Sie den Roboter an einem bestimmten Ort installieren oder Sicherheits-E/A verwenden.

Wichtige Punkte bei der Risikobewertung des Roboterintegrationssystems sind:

* Schweregrad der Kollision durch den Roboter
* Wahrscheinlichkeit einer Kollision durch den Roboter
* Möglichkeit der Kollisionsvermeidung durch den Roboter

Wenn bei der Konfiguration des integrierten Systems die Risikofaktoren durch die sicherheitsrelevanten Funktionen des Roboters nicht ausreichend beseitigt werden können (z. B. Verwendung von Werkzeugen für nicht kollaborative Roboter usw.), müssen Sie durch eine Risikobewertung die erforderlichen zusätzlichen Schutzvorrichtungen installieren.
