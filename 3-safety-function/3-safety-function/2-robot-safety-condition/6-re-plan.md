# 3.3.2.6 Re plan 设置

Re plan 是一个根据从外部安全传感器接收到的信号调整机器人速度的功能。机器人的操作速度根据输入信号的减速率进行调整，TCP 速度在延迟时间后以相应的速度进行监控。

如果延迟时间不足或机器人减速不足，导致违反 TCP 速度限制，则会立即激活安全停止（Stop 0，Stop 1，Stop 2）。

您可以在 `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 6: Re plan]` 菜单中设置参数值。

<p align="center">
<img src="../../../_assets/3/replan_param.png"></img>
<em><p align="center">Re plan 设置界面</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Re plan | <p>是否根据输入信号使用速度控制功能</p><p>(启用 / 禁用)</p> | 禁用 |
| <p>延迟时间</p><p>[ms]</p> | <p>使用 Re plan 时，在延迟时间后监控改变的速度限制值</p><p>(0 ~ 50000)</p> | 2000 |
| <p>速度限制值</p><p>[mm/s]</p> | <p>Re plan 后的 TCP 速度限制值</p><p>(0 ~ 50000)</p> | 50000 |
| <p>速度比例</p><p>[%]</p> | <p>使用 Re plan 时的减速比例</p><p>(0 ~ 100)</p> | 100 |
| <p>输入信号</p><p>[类型, 数字]</p> | <p>Re plan 的输入信号</p><p>( [None, -] / [default input, 3] / [additional input, 0~7] / [safety input, 0~63])</p> | 0 |

{% hint style="warning" %}
<strong>[注意]</strong> 在配置速度限制时，始终考虑停止时间，并覆盖机器人以防止碰撞和伤害。
<strong>[注意]</strong> 高速与大负载成比例于机器人的动能，可能会增加机器人的冲击力。因此，如果机器人与外部物体碰撞，可能会造成重大冲击。在协作空间内保持安全的速度和负载。
{% endhint %}