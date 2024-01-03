# 3.3.2.3 Safety robot modeling

This is the robot model used for safety space monitoring. There are only two safety robot model(:2nd axis and 3rd axis), and the model consits of a capsule.

The capsules used in the safety robot modeling consist of a sphere center and a radius at both ends. The sphere center of the modeling is the robot's 2nd axis/3rd axis center position, and the radius must be large enough to include the size of the current link and the stopping distance at the maximum TCP speed.
 
You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Layout restriction > Robot]** menu.

![Safety robot modeling setting window](../../../_assets/safety_layout/robot_capsule.PNG)


| **Parameter** | 　　　　　　　　　**Description**                                     | **Default setting value** |
| :------: | --------------------------------------------------- | :--------: |
|    Radius    | Radius of model(0 ~ 1000.0 (mm))                           |    0 mm    |
|   Model1  X,Y,Z | Position of center(-1000.0 ~ 1000.0 (mm))                           |    0 mm    |
|   Model2 X,Y,Z | Position of center(-1000.0 ~ 1000.0 (mm))                           |    0 mm    |

{% hint style="warning" %}
**\[Caution]**

* Because the definition of a robot layout setting applies to the 2nd and 3rd axis, the other parts of the robot may intrude into a safety space even if a safety space is set.
{% endhint %}