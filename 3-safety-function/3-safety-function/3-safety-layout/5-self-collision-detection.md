# 3.3.3.5 自我碰撞检测

自我碰撞检测是一种监测机器人第2轴与工具之间潜在碰撞的功能。  
工具与机器人必须按照其实际几何形状进行建模。  
有关建模方法的详细信息，请参阅"[3.3.3.2 安全工具建模](../../../3-safety-function/3-safety-function/3-safety-layout/2-safety-tool-modeling.md)"和"[3.3.3.3 安全机器人建模](../../../3-safety-function/3-safety-function/3-safety-layout/3-safety-robot-modeling.md)"。  

<p align="center">
<img src="../../../_assets/safety_layout/self_collision.png"></img>
<em><p align="center">自我碰撞检测</p></em>
</p>

您可以在`[System > 10: Safety System > 2: Parameter setup > 2: Space restriction > 5: Self-Collision Detection]`菜单中设置机器人的自我碰撞检测功能参数。  

<p align="center">
<img src="../../../_assets/safety_layout/self_collision_param.png"></img>
<em><p align="center">自我碰撞检测功能参数设置屏幕</p></em>
</p>

|  **参数** |                       **描述**                       |  **默认设置**  |
| :-------: | :------------------------------------------------: | :----------: |
| 激活状态 | <p>功能是否被激活</p><p>(无效 / 有效 / 安全 I/O)</p> | 无效 |
| 停止方式 | <p>功能违规时的停止方式</p><p>(停止 0 / 停止 1 / 停止 2 / 不停止)</p> | 停止 1 |