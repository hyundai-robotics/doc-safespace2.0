# 3.3.2.4 TCP orientation monitoring

To use the TCP orientation limiting function in safety tool modeling, you can set cones for monitoring by setting rotation and deviation angles in creating the reference vector.

You can model a cone (![](../../_assets/2.png)) that is formed with generator lines spread by the deviation angle (![](../../_assets/4.png)) from the reference vector (![](../../_assets/3.png)), which is set by the rotation of the Z-direction vector of the robot coordinate system (![](../../_assets/1.png)) at a specified angle. The vertex (![](../../_assets/5.png)) of the cone is located at the TCP, and if the Z-direction vector (![](../../_assets/6.png)) of the TCP exceeds the monitoring cone, a violation error of the TCP position limiting function will occur.

![TCP orientation monitoring](../../../_assets/safety_layout/tool_ori.png)

The safety space can be set from each tab of the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Layout restriction > TCP ]** menu.

![TCP orientation modeling setting window](../../../_assets/safety_layout/tool_ori_param.PNG)


|  **Parameter** |                       **Description**                       |  **Default setting value**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Activation of function</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stop method</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Rx |   <p>Rotation angle of reference vector in X-direction</p><p>(-180.0 ~ 180.0 (deg))</p>  |  0.0 |
| Ry |   <p>Rotation angle of reference vector in Y-direction</p><p>(-180.0 ~ 180.0 (deg))</p>  |  0.0 |
| Rz |   <p>Rotation angle of reference vector in Z-direction</p><p>(-180.0 ~ 180.0 (deg))</p>  |  0.0 |
| Deviation angle |   <p>Limit value of TCP orientation</p><p>(-180.0 ~ 180.0 (deg))</p>  |  0.0 |





{% hint style="warning" %}
**\[Caution]**

* Before changing a tool data, check if the parameters set in the tool modeling are correct. The tool data number and the safety tool modeling number of a tool should be equal to each other.
{% endhint %}
