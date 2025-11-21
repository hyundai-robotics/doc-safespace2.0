# 1.10.3 安全板状态监控

* *\[설정 > 4: 응용 파라미터 > 21: 협동로봇 설정 > 1: 안전 기능 > 5: 안전 상태 모니터링]**请选择*\[设置 > 4: 应用参数 > 21: 协作机器人设置 > 1: 安全功能 > 5: 安全状态监控]菜单的\[SCM状态]**选项卡，确认安全板的状态。**\[SCM 상태]** 탭을 선택하여 안전보드의 상태를 확인하십시오.

![!图15 协作机器人安全状态：SCM状态](../../_assets/image52.jpeg)

* **\[状态]：确认安全状态。**: 안전 상태를 확인합니다.

협동로봇 안전 기능의 상태를 모니터링할 수 있습니다. 정상이면 **可以监控协作机器人安全功能的状态。当为正常时则输出Normal，当安全功能为错误或违规时则可以查看相应的错误代码。**이 출력되고 안전 기능 에러 또는 위반 시에는 해당 에러 코드를 확인할 수 있습니다.


* 确认安全板的状态。
  * **\[Main]：输出SCM的双MCU（MCU A，MCU B）状态**: SCM의 듀얼 MCU (MCU A, MCU B) 상태 출력

POWER\_ON, INIT\_STATE, WAIT\_KIENMATICS\_INFO, WAIT\_DYNAMICS\_INFO, WAIT\_SAFE\_PARAMETER, INITIAL\_MONITORING, NORMAL\_OPERATION, , STO\_STATE\_BY\_PARAM, STO\_STATE\_BY\_SI, SS1\_STATE, SS2\_STATE, SOS\_STATE, FAULT\_STATE
  * **\[编码器]：输出各轴双编码器状态（Normal, Error, Off）**: 축별 듀얼 엔코더 상태 출력(Normal, Error, Off)
  * **\[关节转矩传感器]：输出各轴双JTS状态（Normal, Error, Off）**: 축별 듀얼 JTS 상태 출력(Normal, Error, Off)
