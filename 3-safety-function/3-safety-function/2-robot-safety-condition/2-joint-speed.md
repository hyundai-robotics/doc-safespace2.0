# 3.3.2.2 关节速度限制

关节速度设置参数是监控机器人关节速度的限制值。如果超出限制值，则立即激活指定的安全停机（停止 0、停止 1 或停止 2）。

<p align="center">
<img src="../../../_assets/joint_speed.PNG"></img>
<em><p align="center">关节速度设置示例</p></em>
</p>

您可以在`[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 2: Joint speed]`菜单中设置参数值。

<p align="center">
<img src="../../../_assets/3/joint_speed_set.png"></img>
<em><p align="center">关节速度设置参数设置屏幕</p></em>
</p>

|  **参数** |                       **描述**                       |  **默认设置**  |
| :-------: | :------------------------------------------------: | :----------: |
| 激活 | <p>功能是否激活</p><p>(OFF / ON / Safety I/O)</p> | OFF |
| 停止功能 | <p>功能违反时的停止方式</p><p>(停止 0 / 停止 1 / 停止 2 / 不停止)</p> | 停止 1 |
| 运动调节 | <p>调节为不超过关节速度限制的运动</p><p>(激活 / 禁用)</p> | 禁用 |
| 关节开/关 | <p>每个关节是否激活</p><p>(ON / OFF)</p> | OFF |
| <p>速度</p><p>[mm/s]</p> | <p>每个关节的速度限制</p><p>(10 ~ 10000)</p> | 1000.0 |

{% hint style="warning" %}
<strong>[注意]</strong>: 设置速度监控功能时，务必考虑停止反应时间，并覆盖保护装置以防止碰撞和伤害。
{% endhint %}