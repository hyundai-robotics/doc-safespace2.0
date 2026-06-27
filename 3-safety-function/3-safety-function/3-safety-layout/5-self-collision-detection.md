# 3.3.3.5 自碰撞检测

自碰撞检测是一种监视机器人轴 2 与工具之间潜在碰撞的功能。
工具和机器人必须建模以匹配其实际几何形状。
有关建模方法的详细信息，请参阅"[3.3.3.2 安全工具建模](../../../3-safety-function/3-safety-function/3-safety-layout/2-safety-tool-modeling.md)"和"[3.3.3.3 安全机器人建模](../../../3-safety-function/3-safety-function/3-safety-layout/3-safety-robot-modeling.md)"。

<p align="center">
<img src="../../../_assets/safety_layout/self_collision.png"></img>
<em><p align="center">自碰撞检测</p></em>
</p>

您可以在`[System > 10: Safety System > 2: Parameter setup > 2: Space restriction > 5: Self-Collision Detection]`菜单中设置机器人的自碰撞检测功能参数。

<p align="center">
<img src="../../../_assets/safety_layout/self_collision_param.png"></img>
<em><p align="center">自碰撞检测功能参数设置界面</p></em>
</p>

|  **参数** |                       **描述**                       |  **默认设置**  |
| :-------: | :------------------------------------------------: | :----------: |
| 激活 | <p>功能是否激活</p><p>(无效 / 有效 / 安全 I/O)</p> | 无效 |
| 停止方法 | <p>功能受到违反时的停止方法</p><p>(停止 0 / 停止 1 / 停止 2 / 不停止)</p> | 停止 1 |