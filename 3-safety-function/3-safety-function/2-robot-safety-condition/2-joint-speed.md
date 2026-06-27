# 3.3.2.2 关节速度限制

关节速度设置参数是监测机器人关节速度的限制值。如果违反限制值，则立即激活指定的安全停止（停止 0、停止 1 或停止 2）。

<p align="center">
<img src="../../../_assets/joint_speed.PNG"></img>
<em><p align="center">关节速度设置示例</p></em>
</p>

您可以在`[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 2: Joint speed]`菜单中设置参数值。

<p align="center">
<img src="../../../_assets/3/joint_speed_set.png"></img>
<em><p align="center">关节速度设置参数设置屏幕</p></em>
</p>

|  **参数**  |                       **描述**                       |  **默认设置**  |
| :-------: | :------------------------------------------------: | :----------: |
| 激活 | <p>是否激活该功能</p><p>(OFF / ON / Safety I/O)</p> | OFF |
| 停止功能 | <p>功能被违反时的停止方法</p><p>(停止 0 / 停止 1 / 停止 2 / 不停止)</p> | 停止 1 |
| 运动调节 | <p>调节至不超过关节的速度限制的运动</p><p>(激活 / 禁用)</p> | 禁用 |
| 关节 ON/OFF | <p>每个关节是否被激活</p><p>(ON / OFF)</p> | OFF |
| <p>速度</p><p>[mm/s]</p> | <p>每个关节的速度限制</p><p>(10 ~ 10000)</p> | 1000.0 |

{% hint style="warning" %}
<strong>[警告]</strong>: 设置速度监测功能时，请务必考虑停止反应时间，并覆盖保护罩以防止碰撞和伤害。
{% endhint %}