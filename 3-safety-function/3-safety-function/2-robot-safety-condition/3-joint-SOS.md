# 3.3.2.3 关节停止监控

停止监控在机器人停止操作期间监视每个轴的异常运动。如果违反设定的限制，将立即激活安全停止（停止 0）。

参数值可以在`[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 3: Joint SOS]`菜单中设置。

<p align="center">
<img src="../../../_assets/3/joint_sos.png"></img>
<em><p align="center">停止监控参数设置屏幕</p></em>
</p>

|  **参数** |                       **描述**                       |  **默认设置**  |
| :-------: | :------------------------------------------------: | :----------: |
| 激活 | <p>功能是否激活</p><p>(OFF / ON / Safety I/O)</p> | OFF |
| 关节 ON/OFF | <p>每个关节是否激活</p><p>(ON / OFF)</p> | OFF |
| <p>公差</p><p>[度]</p> | <p>每个关节的角度限制值</p><p>(0.0 ~ 3.0)</p> | 0.100 |

{% hint style="warning" %}
<strong>[注意]</strong>: 如果违反停止监控参数，请在重新启动之前确保机器人运动正常。
{% endhint %}