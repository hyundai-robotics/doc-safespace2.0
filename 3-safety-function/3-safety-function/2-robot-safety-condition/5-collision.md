# 3.3.2.5 碰撞检测

当施加于机器人上的外力超过允许值时，它被识别为碰撞。您可以调整每个轴的灵敏度，灵敏度越高，即使是小的外力也会被识别为碰撞。监测违规时，安全停止（Stop 0，Stop 1，和 Stop 2）会立即激活。

`[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 5: Collision detection]` 菜单允许您设置参数值。

<p align="center">
<img src="../../../_assets/3/collision.png"></img>
<em><p align="center">碰撞检测参数设置屏幕</p></em>
</p>

| **参数** |                             **描述**                             |  **默认设置**  |
| :------: | :----------------------------------------------------------: | :---------: |
| 激活   | <p>功能激活状态</p><p>(OFF/ON/Safety Input)</p>     |   OFF  |
| 停止功能 |   <p>功能违规时的停止方法</p><p>(Stop 0, Stop 1, Stop 2, Non-stop)</p>  | Stop 1 |
| 关节 ON/OFF |   <p>每个关节的激活状态</p><p>(ON/OFF)</p>  |  OFF |
| 灵敏度  |   <p>每个关节的检测灵敏度</p><p>(1 ~ 200(%))</p>  |  100 |

{% hint style="warning" %}
<strong>[警告]</strong> 由于机器人在高速和大负载时的冲击力可能与动能成正比，因此如果机器人与外部物体发生碰撞，可能会产生相当大的冲击。在协作空间中，在保持安全速度和负载的情况下操作。
<strong>[警告]</strong> 如果工具信息和附加重量设置与实际值不同，可能会发生误检。在使用碰撞检测功能之前，请检查每个信息。
{% endhint %}