# 3.3.2.2 Safety tool modeling

Safety space monitoring detects whether the tool modeled in spheres intrudes into the safety spaces or exceeds the working space. You can set up to 16 safety tools and model a safety tool with a maximum of 10 spheres.

Because a safety tool is enabled by a number that is set on the teach pendant, you should model a safety tool based on the tool data set in the **\[Setting > 3: Robot parameter > 1: Tool data**] menu. Refer to the TCP position information displayed at the top of the tool data setting window.

There are 3 modles fot modleing safety tool: shpere, capsule and rounded plate. Each safety tool modeling is set by its center and radius. Set the center position of the sphere for the modeling based on the robot flange coordinate system (Xf, Yf, and Zf), and set the radius of the sphere, including the tool size and the stopping distance, at the maximum TCP speed.

![Tool modeling](../../../_assets/safety_layout/tool_sphere.PNG)

![Robot flange coordinate system](../../../_assets/safety_layout/flange.PNG)


You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Layout restriction > Tool]** menu.

![Safety tool modeling setting window](../../../_assets/safety_layout/tool_sphere.PNG)


|  **Parameter** |                       **Description**                       |  **Default setting value**  |
| :-------: | :------------------------------------------------: | :----------: |
| TCP X,Y,Z | <p>TCP position in flange coordination(read only)- set in Tool data menu</p> |   0  |
| Shape |   <p>Type of modeling shape</p><p>(Off/sphere/capsule/R-plate)</p>  | Off |
| Radius |  <p>Radius of model</p><p>(0.0 ~ 1000.0 mm)</p>  | 0 |
| Height |  <p>Height of R-plate</p><p>(0.0 ~ 1000.0 mm)</p>  | 0 |
| Width |  <p>Width of R-plate</p><p>(0.0 ~ 1000.0 mm)</p>  | 0 |
| X |  <p>Position of center in X direction</p><p>(-1000.0 ~ 1000.0 mm)</p>  | 0 |
| Y |  <p>Position of center in Y direction</p><p>(-1000.0 ~ 1000.0 mm)</p>  | 0 |
| Z |  <p>Position of center in Z direction</p><p>(-1000.0 ~ 1000.0 mm)</p>  | 0 |





{% hint style="warning" %}
**\[Caution]**

* Before changing a tool data, check if the parameters set in the tool modeling are correct. The tool data number and the safety tool modeling number of a tool should be equal to each other.
* Because the definition of a robot layout setting applies to the 2nd and 3rd axis, the other parts of the robot may intrude into a safety space even if a safety space is set.
{% endhint %}
