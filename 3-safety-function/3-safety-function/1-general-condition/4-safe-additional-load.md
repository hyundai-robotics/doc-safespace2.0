# 3.3.1.4 Safety Added Weight

Safety added weight information is used by the safety board to calculate the robot's torque. You must enter the information for the added weight actually installed on the robot. The information must be identical to the added weight information used for robot control (**\[System > 3: Robot Parameters > 7: Added Weight by Axis]**).


* **\[System > 8: Safety System > 1: Basic Settings > 4: Safety Additional Weight]** You can set the safety additional weight information in the menu, and you can load the additional weight information used for robot control by clicking "Load Additional Weight" at the bottom of the menu.


<p align="center">
<img src="../../../_assets/3/add_tool_param.png"></img>
<em><p align="center">Safety Added weight parameter setting screen</p></em>
</p>


|  **Parameter** |                       **Description**                       |  **Default value**  |
| :-------: | :------------------------------------------------: | :-------------: |
| <p>Weight</p><p>[kg]</p> | <p>Weight of the tool</p><p>(0.0 ~ 1000.0)</p> | 0.0 |
| <p>Center</p><p>[mm]</p> | <p>Position of the center of gravity of the tool relative to the center of the flange</p><p>(-3000.0 ~ 3000.0)</p> | 0.0 |
| <p>Inertia</p><p>[kg·㎡]</p> | <p>Moment of inertia of the tool with respect to the tool coordinates</p><p>(0.0 ~ 2000.000)</p> | 0.0 |
| Load Additional Weight | A function to load additional weight information used for robot control | - |
| Copy | A function to copy the values   entered on the corresponding page | - |
| Paste | A function to paste the values   from the copied page onto the corresponding page | - |

{% hint style="warning" %}
**\[Caution]**: If the safety weight information and the weight information used for robot control do not match, a warning/error will occur and the robot will not be able to operate. Be sure to match the weight information with the actual attached weight before operating the robot. 
{% endhint %}
 
{% hint style="warning" %}
**\[Caution]**: The safety additional weight number is supported from 0 to 2, and each number matches the axis number of the system additional weight (0-S axis, 1-H axis, 2-V axis). Please enter the additional weight information by matching the safety parameter number with the axis number.
{% endhint %}
 
 