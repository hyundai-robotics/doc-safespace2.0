# 3.3.2.8 动量设置

此功能监控机器人产生的动量是否超过允许限值。如果发生监控违规，将立即激活安全停止（Stop 0、Stop 1或Stop 2）。

您可以在`[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 8: Momentum]`菜单中设置参数值。

<p align="center">
<img src="../../../_assets/3/momentum.png"></img>
<em><p align="center">动量设置界面</p></em>
</p>

| **参数**    |          **描述**                                                  |  **默认设置** |
| :------: | :----------------------------------------------------------------: | :---------: |
| 激活         | <p>功能是否激活</p><p>(OFF / ON / Safety I/O)</p>              | OFF |
| 停止功能     | <p>功能违规时的停止方法</p><p>(Stop 0 / Stop 1 / Stop 2 / No stop)</p> | Stop 1 |
| 运动调节      | <p>调节到不超过机器人动量限制的运动</p><p>(Enable / Disable)</p> | Disable |
| <p>最大动量</p><p>[kg m/s]</p> | <p>机器人的动量限值</p><p>(5 ~ 50000)</p> | 1000 |

{% hint style="warning" %}
<strong>[注意]</strong> 高速和大负载与机器人的动能成正比，可能增加机器人的冲击力。因此，与外部物体发生碰撞可能导致重大影响。在协作空间中，请保持安全速度和负载。
<strong>[注意]</strong> 设置工具信息和额外重量与实际值不同可能导致错误检测。使用此功能前请检查信息。
{% endhint %}