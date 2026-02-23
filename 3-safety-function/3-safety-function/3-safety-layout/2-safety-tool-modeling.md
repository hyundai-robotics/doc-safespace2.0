# 3.3.2.2 Safety Tool Modeling

Monitors whether the sphere modeled with a tool used for safety area monitoring violates the protected space or leaves the work space. Up to 16 safety tools can be set and modeled with up to 10 models.

As the safety tool is activated by the tool number set on the teach pendant, you should model the safety tool based on the tool data set in the `[System > 3: Robot Parameters > 1: Tool Data]` menu. Refer to the TCP position information at the top of the tool data setting screen.

There are a total of 3 models used for safety tool modeling: sphere, capsule, and plate. Each model consists of a center and radius. The center position and radius of the modeling are set based on the robot flange coordinate system (Xf, Yf, and Zf), and the radius is set to include the tool size and stop distance at maximum TCP speed.

<p align="center">
<img src="../../../_assets/safety_layout/tool_model.png"></img>
<em><p align="center">Tool modeling</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **shape**  |
| :-------: | :------------------------------------------------: | :----------: |
| c | center(X,Y,Z based robot flange coordinate system) |   sphere, capsule, plate  |
| r | radius  |   sphere, capsule, plate  |
| h | height  |   capsule, plate  |
| w | width  |   plate  |

<p align="center">
<img src="../../../_assets/safety_layout/flange.png"></img>
<em><p align="center">Robot flange coordinate system</p></em>
</p>

You can set parameter values   in the `[System > 8: Safety System > 2: Parameter Setting > 2: Area Limit > 3: Tool Modeling]` menu.

<p align="center">
<img src="../../../_assets/safety_layout/tool_param.png"></img>
<em><p align="center">Safety Tool Modeling Settings Screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| TCP X,Y,Z | <p>TCP position in flange coordinate system (read-only) - set in tool info</p> | 0 |
| Geometry | <p>Tool modeling shape</p><p>(off / sphere / capsule / plate)</p> | off |
| <p>Radius</p><p>[mm]</p> | <p>Radius</p><p>(0.0 ~ 3000.0)</p> | 0 |
| <p>Height</p><p>[mm]</p> | <p>Height of plate</p><p>(0.0 ~ 5000.0)</p> | 0 |
| <p>Width</p><p>[mm]</p> | <p>Width of plate</p><p>(0.0 ~ 5000.0)</p> | 0 |
| <p>X</p><p>[mm]</p> | <p>Model center position in X direction</p><p>(-5000.0 ~ 5000.0)</p> | 0 |
| <p>Y</p><p>[mm]</p> | <p>Model center position in Y direction</p><p>(-5000.0 ~ 5000.0)</p> | 0 |
| <p>Z</p><p>[mm]</p> | <p>Model center position in Z direction</p><p>(-5000.0 ~ 5000.0)</p> | 0 |
| <p>Rot.X</p><p>[deg]</p> | <p>X direction in flange coordinate system</p><p>(-180.0 ~ 180.0)</p> | 0 |
| <p>Rot.Y</p><p>[deg]</p> | <p>Y direction in flange coordinate system</p><p>(-180.0 ~ 180.0)</p> | 0 |
| <p>Rot.Z</p><p>[deg]</p> | <p>Z direction in flange coordinate system</p><p>(-180.0 ~ 180.0)</p> | 0 |





{% hint style="warning" %}
**\[Caution]**

* When changing tool data, be sure to recheck that the parameters set in safety tool modeling are accurate. The tool data number and safety tool modeling number of the same tool should match.
* As the definition of robot layout settings applies only to the robot 2nd and 3rd axes, other parts of the robot may violate this area even if a safety area is set.
{% endhint %}
