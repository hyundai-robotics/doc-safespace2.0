# 3.3.3.5 Self-Collision Detection

Self-collision detection is a function that monitors potential collisions between Axis 2 of the robot and the tool.
The tool and the robot must be modeled to match their actual geometries.
For detailed information on the modeling methods, refer to "[3.3.3.2 Safety Tool Modeling](../../../3-safety-function/3-safety-function/3-safety-layout/2-safety-tool-modeling.md)" and "[3.3.3.3 Safety Robot Modeling](../../../3-safety-function/3-safety-function/3-safety-layout/3-safety-robot-modeling.md)".

<p align="center">
<img src="../../../_assets/safety_layout/self_collision.png"></img>
<em><p align="center">Self-Collision Detection</p></em>
</p>


You can set parameters for the robot's self-collision detection function in the `[System > 8: Safety System > 2: Parameter Settings > 2: Area Limits > 5: Self-Collision Detection]` menu.

<p align="center">
<img src="../../../_assets/safety_layout/self_collision_param.png"></img>
<em><p align="center">Self-collision detection function parameter setting screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Whether the function is activated</p><p>(Invalid / Valid / Safe I/O)</p> | Invalid |
| Stop method | <p>Stop method when the function is violated</p><p>(Stop 0 / Stop 1 / Stop 2 / No stop)</p> | Stop 1 |




