# 1.3.1 Roboterbeschränkungsfunktion

Die Roboterbeschränkungsfunktion begrenzt die Bewegung des Roboters in der Sicherheitszone und unterstützt die folgenden Funktionen:

* **TCP-Position: Verhindert, dass das Werkzeug oder der Ellbogen des Roboters, modelliert als Kugel, die festgelegte Zone verletzt oder verlässt.**: 로봇의 툴 또는 엘보우를 구로 모델링한 형상이 설정한 영역으로 침범하거나 벗어나는 것을 제한

***
* **TCP-Orientierung: Verhindert, dass die Endeffektor- und Werkzeugorientierung den festgelegten Orientierungsbereich verlässt.**: 로봇의 엔드 이펙터와 툴이 향하는 방향이 설정한 방향의 범위를 벗어나는 것을 제한

***
* **TCP-Geschwindigkeit: Begrenzt die Geschwindigkeit des Roboters auf eine niedrige Geschwindigkeit, um genügend Zeit zu haben, um eine Kollision zwischen dem Roboter und dem Arbeiter zu vermeiden (arbeitet im manuellen Modus mit maximal 250 mm/s oder weniger).**: 로봇과 작업자의 충돌을 피할 시간을 확보하도록 로봇의 속도를 저속으로 제한(수동 모드에서는 최대 250 ㎜/sec 이하로 동작)

***
* **TCP-Kraft, Leistung, Kollisionserkennung: Begrenzt Kraft und Druck im Falle einer Kollision zwischen dem Roboter und dem Arbeiter.**: 로봇과 작업자의 충돌 발생 시의 힘과 압력을 제한

***
* **Momentum: Begrenzt Energie und Aufprallbelastung im Falle einer Kollision zwischen Roboter und Arbeiter**: 로봇과 작업자의 충돌 발생 시의 에너지와 충격 하중을 제한
