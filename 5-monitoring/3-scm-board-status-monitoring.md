# 1.10.3 安全板状态监测

选择 **\[Settings > 4: Application Parameters > 21: Collaborative Robot Setup > 1: Safety Function > 5: Safety Status Monitoring]** 菜单的 **\[SCM Status]** 选项卡以检查安全板的状态。

![!Figure 15 Collaborative Safety Status: SCM Status](../../_assets/image52.jpeg)

* **\[Status]**: 检查安全状态。

  您可以监测协作机器人安全功能的状态。当功能正常时输出 **Normal**，发生安全功能错误或违规时您可以检查相应的错误代码。


* 检查安全板的状态。
  * **\[Main]**: SCM 双 MCU (MCU A, MCU B) 状态输出

    POWER\_ON, INIT\_STATE, WAIT\_KIENMATICS\_INFO, WAIT\_DYNAMICS\_INFO, WAIT\_SAFE\_PARAMETER, INITIAL\_MONITORING, NORMAL\_OPERATION, , STO\_STATE\_BY\_PARAM, STO\_STATE\_BY\_SI, SS1\_STATE, SS2\_STATE, SOS\_STATE, FAULT\_STATE
  * **\[Encoder]**: 按轴的双编码器状态输出（正常，错误，关闭）
  * **\[Joint Torque Sensor]**: 按轴的双 JTS 状态输出（正常，错误，关闭）