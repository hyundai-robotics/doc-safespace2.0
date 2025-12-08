# 1.10.3 Safety Board Status Monitoring

Select the **\[Settings > 4: Application Parameters > 21: Collaborative Robot Setup > 1: Safety Function > 5: Safety Status Monitoring]** menu's **\[SCM Status]** tab to check the status of the safety board.

![!Figure 15 Collaborative Safety Status: SCM Status](../../_assets/image52.jpeg)

* **\[Status]**: Check the safety status.

  You can monitor the status of collaborative robot safety function. **Normal** is output when the function normal, and you can check the corresponding error code when a safety function error or violation occurs.


* Check the status of the safety board.
  * **\[Main]**: SCM dual MCU (MCU A, MCU B) status output

    POWER\_ON, INIT\_STATE, WAIT\_KIENMATICS\_INFO, WAIT\_DYNAMICS\_INFO, WAIT\_SAFE\_PARAMETER, INITIAL\_MONITORING, NORMAL\_OPERATION, , STO\_STATE\_BY\_PARAM, STO\_STATE\_BY\_SI, SS1\_STATE, SS2\_STATE, SOS\_STATE, FAULT\_STATE
  * **\[Encoder]**: Dual encoder status output by axis (Normal, Error, Off)
  * **\[Joint Torque Sensor]**: Dual JTS status output by axis (Normal, Error, Off)
