# 1.10.3 安全板状态监控

请选择 **\[设置 > 4: 应用参数 > 21: 协作机器人设置 > 1: 安全功能 > 5: 安全状态监控]** 菜单的 **\[SCM状态]** 选项卡，确认安全板的状态。

![!图15 协作机器人安全状态：SCM状态](../../_assets/image52.jpeg)

* **\[状态]**：确认安全状态。

  可以监控协作机器人安全功能的状态。当为正常时则输出Normal，当安全功能为错误或违规时则可以查看相应的错误代码。


* 确认安全板的状态。
  * **\[主要的]**：输出SCM的双MCU（MCU A，MCU B）状态

    POWER\_ON, INIT\_STATE, WAIT\_KIENMATICS\_INFO, WAIT\_DYNAMICS\_INFO, WAIT\_SAFE\_PARAMETER, INITIAL\_MONITORING, NORMAL\_OPERATION, , STO\_STATE\_BY\_PARAM, STO\_STATE\_BY\_SI, SS1\_STATE, SS2\_STATE, SOS\_STATE, FAULT\_STATE
  * **\[编码器]**：输出各轴双编码器状态（Normal, Error, Off）
  * **\[关节转矩传感器]**：输出各轴双JTS状态（Normal, Error, Off）
