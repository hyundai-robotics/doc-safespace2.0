# 3.3.3.1 Safety Area Setting

A safety area is a work space or protected space for monitoring the tool and robot link areas. The work space is a restricted space where the monitored object can move freely but cannot leave. In contrast, the protected space is a restricted space where the monitored object cannot move once it enters. If the robot leaves the set work space or violates the protected space, a safety stop (Stop 0, Stop 1, and Stop 2) is activated.

<p align="center">
<img src="../../../_assets/safety_layout/cell_general.png"></img>
<em><p align="center">work space</p></em>
</p>

<p align="center">
<img src="../../../_assets/safety_layout/cell_protected.png"></img>
<em><p align="center">protected space</p></em>
</p>

The safe zone is configured by setting the position and height of each vertex relative to the robot's coordinate system. Up to 10 vertices can be added. The safe zone is activated by parameter settings or safety input/output signals.

You can set the parameter values   for the safety zone in each tab of the `[System > 10: Safety System > 2: Parameter Setup > 2: Space restriction > 1: Space]` menu.


* **General**

<p align="center">
<img src="../../../_assets/safety_layout/cell_general.png"></img>
<em><p align="center">General</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Function activation status</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stop method when the function is violated</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Type |  <p>Safety area type</p><p>(Work space/Protected space)</p>  | Work space |


* **Detection target**

<p align="center">
<img src="../../../_assets/safety_layout/cell_target.png"></img>
<em><p align="center">Detection target</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Tool | <p>Tool modeling monitoring</p><p>(Off/On/Safety Input)</p> |   Off  |
| Lower arm |   <p>Robot 2nd axis modeling monitoring</p><p>(Off/On)</p>  | Off |
| Upper arm |  <p>Robot 3rd axis modeling monitoring</p><p>(Off/On)</p>  | Off |


* **Area**

<p align="center">
<img src="../../../_assets/safety_layout/cell_working.png"></img>
<em><p align="center">Area</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| <p>Z Min / Max</p><p>[mm]</p> | <p>Height of the safe area based on the robot coordinate system</p><p>(-5000.0 ~ 5000.0)</p> | 0 |
| Enable | <p>Whether to enable the vertex of the safe area</p><p>(Enable / Disable)</p> | Disable |
| <p>X</p><p>[mm]</p> | <p>X-direction position of the vertex based on the robot coordinate system</p><p>(-5000.0 ~ 5000.0)</p> | 0 |
| <p>Y</p><p>[mm]</p> | <p>Y-direction position of the vertex based on the robot coordinate system</p><p>(-5000.0 ~ 5000.0)</p> | 0 |



{% hint style="warning" %}
**\[Caution]**: The safety function monitors based on the set area. The set area should be configured considering the stop distance, and verification must be performed before operation.
{% endhint %}