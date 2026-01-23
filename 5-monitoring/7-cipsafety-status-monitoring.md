# 5.4 CIP Safety Monitoring

You can monitor the I/O status of CIP Safety by navigating to the **[System > 2: Control Parameters > 11: Industrial Communication > 6: Safety Communication > 3: CIP Safety]** menu.

<p align="center">
<img src="../_assets/cipSafety/cipsafety_status.png"></img>
<em><p align="center">CIP Safety Monitoring</p></em>
</p>

- **Device Status:** <br>
Executing : CIP Safety communication is running. <br>
Idle : CIP Safety application is running, but CIP Safety communication has not started. <br>
Abort : Initial step Error<br>
Fault : Critical Error<br>
Configuring : Applying Configuration data failed<br>
- **Communication Status:**<br>
Connection Fail : A connection failure has occurred.
On-Line, Connected : Link is OK. The device is online and connected to Originator.
On-Line, No Conn : The device is online but not connected to Originator.
- **I/O Count:** (Number of I/O transmissions/receptions)
