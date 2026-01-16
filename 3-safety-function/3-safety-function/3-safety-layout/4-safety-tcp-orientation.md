# 3.3.2.4 TCP Orientation Monitoring

To use the TCP orientation monitoring function, you can set up a monitoring cone by setting the rotation angle and deviation angle for generating the reference vector.

By setting the reference vector (![](../../../_assets/3.png)) by rotating the Z-direction vector of the robot coordinate system (![](../../../_assets/1.png)) by a set angle based on it, a cone (![](../../../_assets/2.png)) made up of mother lines that are separated by the deviation angle (![](../../../_assets/4.png)) can be modeled. The vertex of such a cone (![](../../../_assets/5.png)) is located at the TCP, and if the Z-direction vector of the TCP (![](../../../_assets/6.png)) crosses the monitoring cone, a TCP direction limit function violation error occurs.

<p align="center">
<img src="../../../_assets/safety_layout/tool_ori.png"></img>
<em><p align="center">TCP Orientation Monitoring</p></em>
</p>

You can set the parameter values ​​in the **\[System > 8: Safety System > 2: Parameter Setting > 2: Area Limit > 4: Tool Direction]** menu.

<p align="center">
<img src="../../../_assets/safety_layout/tool_orient.png"></img>
<em><p align="center">TCP Orientation parameter setting screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Whether the function is activated</p><p>(Invalid / Valid / Safe I/O)</p> | Invalid |
| Stop method | <p>Stop method in case of function violation</p><p>(Stop 0 / Stop 1 / Stop 2 / No stop)</p> | Stop 1 |
| <p>Org.Rx</p><p>[deg]</p> | <p>Rotation amount of reference vector relative to X direction</p><p>(-180.0 ~ 180.0)</p> | 0.0 |
| <p>Org.Ry</p><p>[deg]</p> | <p>Rotation amount of reference vector relative to Y direction</p><p>(-180.0 ~ 180.0)</p> | 0.0 |
| <p>Org.Rz</p><p>[deg]</p> | <p>Rotation of reference vector relative to Z direction</p><p>(-180.0 ~ 180.0)</p> | 0.0 |
| Deviation angle | <p>Tool orientation limit</p><p>(-180.0 ~ 180.0)</p> | 0.0 |
| Load current position <br> | Create reference vector with current robot pose | - |


{% hint style="warning" %}
**\[Caution]**

* When changing tool data, be sure to recheck that the parameters set in safety tool modeling are accurate. The tool data number and safety tool modeling number of the same tool should match.
{% endhint %}
