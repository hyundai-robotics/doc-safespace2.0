# 3.3.3.1 Sicherheits-Eingangs-/Ausgangssignale

Legen Sie die Parameter für die Sicherheits-Eingangs-/Ausgangssignale fest.
Es gibt 4 Eingangssignale und 1 Ausgangssignal, die alle als Doppelsignale fungieren.


## 1. Eingangssignaleinstellungen

![!Default Input Image](../../../_assets/safety_io/def_input.PNG)

- **- Impulstest: Legen Sie fest, ob für jeden Kanal ein Impulstest verwendet werden soll.** : 각 채널별로 Pulse Test 사용 여부를 설정합니다.
- **- Fehlerhaltezeit: Wenn in einem Kanal ein Fehler auftritt, wechselt das System nach Ablauf der eingestellten Zeit vom Fail-Safe-Zustand in den aktuellen Eingangsstatus, selbst wenn der Fehler behoben wurde. (Einheit: ms)** : 해당 채널에서 에러가 발생하면, 에러가 복구되더라도 설정된 시간 이후에 Fail-Safe 상태에서 현재 입력 상태로 전환됩니다. (단위 : msec)
- **- Filterzeit: Das gleiche Signal muss für die für jeden Kanal eingestellte Filterzeit eingegeben werden, damit es als gültiges Signal verarbeitet wird. (Einheit: ms)** : 각 채널별로 설정된 **- Filterzeit: Das gleiche Signal muss für die für jeden Kanal eingestellte Filterzeit eingegeben werden, damit es als gültiges Signal verarbeitet wird. (Einheit: ms)** 동안 동일한 신호가 입력되어야 유효한 신호로 처리됩니다. (단위 : msec)
- **- Diskrete Zeit: Das grundlegende Eingangssignal wird als gültig verarbeitet, wenn zwei Doppelsignale identisch sind. Wenn die beiden Signale länger als die eingestellte diskrete Zeit voneinander abweichen, wird ein Alarm ausgelöst. (Einheit: ms)** : 기본 입력 신호는 두 개의 이중 신호가 동일할 때 유효한 신호로 처리됩니다. 두 신호가 설정된 **- Diskrete Zeit: Das grundlegende Eingangssignal wird als gültig verarbeitet, wenn zwei Doppelsignale identisch sind. Wenn die beiden Signale länger als die eingestellte diskrete Zeit voneinander abweichen, wird ein Alarm ausgelöst. (Einheit: ms)** 이상 서로 다르면 알람이 발생합니다. (단위 : msec)


## 2. Ausgangssignaleinstellungen

![!Default Output Image](../../../_assets/safety_io/def_output.PNG)

- **- Impulstest: Legen Sie fest, ob für jeden Kanal ein Impulstest verwendet werden soll.** : 각 채널별로 Pulse Test 사용 여부를 설정합니다.
- **- Fehlerhaltezeit: Wenn im Kanal ein Fehler auftritt, bleibt der Ausgangskontakt für die eingestellte Zeiti m Zustand „Offen“ (Fail-Safe), auch wenn der Fehler behoben wurde. Danach wechselt er in den normalen Ausgangszustand. (Einheit: ms)** : 해당 채널에서 에러가 발생하면, 에러가 복구되더라도 설정된 시간 동안 출력 접점은 **- Fehlerhaltezeit: Wenn im Kanal ein Fehler auftritt, bleibt der Ausgangskontakt für die eingestellte Zeiti m Zustand „Offen“ (Fail-Safe), auch wenn der Fehler behoben wurde. Danach wechselt er in den normalen Ausgangszustand. (Einheit: ms)** 상태를 유지합니다. 이후 정상 출력으로 전환됩니다. (단위 : msec)
