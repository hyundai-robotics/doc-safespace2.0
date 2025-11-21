# 3.3.3.2 Zusätzliche Sicherheits-Eingangs-/Ausgangssignale

Legen Sie Parameter für zusätzliche Sicherheits-Eingangs-/Ausgangssignale fest.
Besteht aus 8 Eingangssignalen und 8 Ausgangssignalen, die alle als Doppelsignale fungieren.

## 1. Zusätzliche Sicherheits-Eingangs-/Ausgangssignale

![!Additional Input Image](../../../_assets/safety_io/add_io.PNG)

- **- Aktivieren: Nicht verwendet** : 미사용
- **- Filterzeit: Für jeden Eingangskanal muss während der Filterzeit ein konstantes Signal eingegeben werden, damit es als gültiges Signal verarbeitet wird. (Einheit: ms)** : 각 입력 채널별로 필터 시간 동안 일정한 신호가 입력되어야 유효한 신호로 처리됩니다. (단위 : msec)
- **- Diskrete Zeit: Der zusätzliche Sicherheitseingang wird als gültiges Signal verarbeitet, wenn zwei Doppelsignale denselben Wert haben. Wenn diese beiden Signale länger als die diskrete Zeit voneinander abweichen, wird ein Alarm ausgelöst. (Einheit: ms)** :  Additional Safety Input 은 2개의 이중 신호가  같은 값일때 유효한 신호로 처리되고 이 2개의 신호가 **- Diskrete Zeit: Der zusätzliche Sicherheitseingang wird als gültiges Signal verarbeitet, wenn zwei Doppelsignale denselben Wert haben. Wenn diese beiden Signale länger als die diskrete Zeit voneinander abweichen, wird ein Alarm ausgelöst. (Einheit: ms)** 보다 큰 시간 동안 다르게 되면 알람이 발생하게 됩니다. (단위 : msec)
- **- Haltezeit für Eingangsfehler (Input Error Latch Time): Wenn in einem Kanal ein Fehler auftritt, wechselt das System nach Ablauf der eingestellten Zeit vom Fail-Safe-Zustand in den aktuellen Eingangsstatus, selbst wenn der Fehler behoben wurde. (Einheit: ms)** :  해당 채널에서 에러가 발생하면, 에러가 복구되더라도 설정된 시간 이후에 Fail-Safe 상태에서 현재 입력 상태로 전환됩니다. (단위 : msec)
- **- Haltezeit für Ausgangsfehler (Output Error Latch Time): Wenn im Kanal ein Fehler auftritt, bleibt der Ausgangskontakt für die eingestellte Zeiti m Zustand „Offen“ (Fail-Safe), auch wenn der Fehler behoben wurde. Danach wechselt er in den normalen Ausgangszustand. (Einheit: ms)** : 해당 채널에서 에러가 발생하면, 에러가 복구되더라도 설정된 시간 동안 출력 접점은 **- Haltezeit für Ausgangsfehler (Output Error Latch Time): Wenn im Kanal ein Fehler auftritt, bleibt der Ausgangskontakt für die eingestellte Zeiti m Zustand „Offen“ (Fail-Safe), auch wenn der Fehler behoben wurde. Danach wechselt er in den normalen Ausgangszustand. (Einheit: ms)** 상태를 유지합니다. 이후 정상 출력으로 전환됩니다. (단위 : msec)
 

