# 5.4 CIP Safety Monitoring

您可以通过导航到 `[System > 2: Control Parameters > 11: Industrial Communication > 6: Safety Communication > 3: CIP Safety]` 菜单来监控 CIP Safety 的 I/O 状态。

<p align="center">
<img src="../_assets/cipSafety/cipsafety_status.png"></img>
<em><p align="center">CIP Safety Monitoring</p></em>
</p>

- **Device Status:** <br>
执行中 : CIP Safety 通信正在运行。 <br>
空闲 : CIP Safety 应用程序正在运行，但 CIP Safety 通信尚未开始。 <br>
中止 : 初始步骤错误<br>
故障 : 严重错误<br>
配置中 : 应用配置数据失败<br>
- **Communication Status:**<br>
连接失败 : 发生连接失败。
在线，已连接 : 链接正常。设备在线并已连接到发起者。
在线，未连接 : 设备在线但未连接到发起者。
- **I/O Count:** (I/O 传输/接收数量)