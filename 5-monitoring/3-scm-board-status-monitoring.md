# 1.10.3 安全板状态监控

选择 **\[设置 > 4: 应用参数 > 21: 协作机器人设置 > 1: 安全功能 > 5: 安全状态监控]** 菜单的 **\[SCM 状态]** 标签以检查安全板的状态。

![!Figure 15 协作安全状态: SCM 状态](../../_assets/image52.jpeg)

* **\[状态]**: 检查安全状态。

  您可以监控协作机器人安全功能的状态。当功能正常时，输出 **正常**，并且在发生安全功能错误或违规时，您可以检查相应的错误代码。

  
* 检查安全板的状态。
  * **\[主]**: SCM 双 MCU (MCU A, MCU B) 状态输出

    POWER\_ON, INIT\_STATE, WAIT\_KIENMATICS\_INFO, WAIT\_DYNAMICS\_INFO, WAIT\_SAFE\_PARAMETER, INITIAL\_MONITORING, NORMAL\_OPERATION, , STO\_STATE\_BY\_PARAM, STO\_STATE\_BY\_SI, SS1\_STATE, SS2\_STATE, SOS\_STATE, FAULT\_STATE
  * **\[编码器]**: 按轴的双编码器状态输出 (正常, 错误, 关闭)
  * **\[关节扭矩传感器]**: 按轴的双 JTS 状态输出 (正常, 错误, 关闭)