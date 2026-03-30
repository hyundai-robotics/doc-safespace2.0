# 3.3.2.5 碰撞检测

当施加在机器人上的外部力超过允许值时，它被识别为碰撞。您可以调整每个轴的灵敏度，灵敏度越高，即使是小的外部力也会被识别为碰撞。当监控被违反时，安全停止（Stop 0、Stop 1 和 Stop 2）会立即被激活。

`[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 5: Collision detection]` 菜单允许您设置参数值。

<p align="center">
<img src="../../../_assets/3/collision.png"></img>
<em><p align="center">碰撞检测参数设置屏幕</p></em>
</p>

| **参数** |                                  **描述**                                  |  **默认设置** |
| :------: | :----------------------------------------------------------------: | :---------: |
| 激活 | <p>功能激活状态</p><p>(OFF/ON/Safety Input)</p> |   OFF  |
| 停止功能 |   <p>当功能被违反时的停止方法</p><p>(Stop 0, Stop 1, Stop 2, Non-stop)</p>  | Stop 1 |
| 关节 ON/OFF |   <p>每个关节的激活状态</p><p>(ON/OFF)</p>  |  OFF |
| 灵敏度 |   <p>每个关节的检测灵敏度</p><p>(0 ~ 200(%))</p>  |  100 |

{% hint style="warning" %}
<strong>[注意]</strong> 由于在高速和大负载时机器人的冲击力会随动能成比例增加，如果机器人与外部物体碰撞，可能会产生较大的冲击。在协作空间中，操作时请保持安全的速度和负载。
<strong>[注意]</strong> 如果工具信息和附加重量的设置与实际值不同，可能会发生错误检测。在使用碰撞检测功能之前，请检查每条信息。
{% endhint %}