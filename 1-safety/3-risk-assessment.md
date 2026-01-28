# 1.3 Risk Assessment

In the integrated system configuration including the robot, risk assessment is one of the important factors that is handled as a legal requirement in most countries. As the safety assessment for robot installation varies depending on how the robot is integrated into the system, the risk of the integrated system cannot be assessed with the robot alone.

The system administrator should configure and operate the system according to the guidelines of ISO 12100 and ISO 10218-2 to conduct a risk assessment. You can also refer to the technical specification ISO/TS 15066.

Conduct a risk assessment considering the entire process of the integrated system including the robot. The main goals of risk assessment are as follows:

* Basic settings for robot use and robot teaching
* Problem diagnosis and maintenance
* Normal operation of the installed robot

After installing the robot and configuring the system, you must conduct a risk assessment. The risk assessment mainly determines the appropriateness of the safety devices in the integrated robot system, as well as the need for additional emergency stop devices and other safety devices.

It is very important to identify appropriate safety devices and properly configure an integrated robot system. Configure an integrated system by referring to relevant contents in the manual.

You can set limits for the robot's TCP speed, pressure, power, momentum, collision detection, reduction ratio, joint angle by axis, speed, etc. You can also configure safety functions using safety-related I/O and communication. For detailed information on the configuration of safety functions, refer to "[3. SafeSpace2.0 Safety Functions](../3-safety-function/README.md)".

**\[Safety Function]** menu allows you to configure safety-related functions, and the available functions are as follows:

* **Force and Power Limit**: Restricts the force and pressure for stopping in preparation for collision between the robot and the worker
* **Momentum Limit**: Reduces the robot's operating speed to limit energy and impact load in preparation for collision between the robot and the worker
* **Joint and TCP Position Limit**: Restricts movement to prevent the robot from moving to specific body parts such as the user's neck or head
* **TCP and Tool Posture Limit**: Restricts movement to reduce risks related to specific areas or features of the tool and workpiece (e.g., to prevent sharp parts of the tool or workpiece from moving toward the worker)
* **Speed Limit**: Restricts the robot's movement to remain at low speed to provide time for the worker to avoid collision in preparation for collision between the robot and worker

In addition, you can configure safety-related functions by installing the robot in a specific location or using safety I/O.

Important items when conducting risk assessment of the integrated robot system are as follows:

* Collision severity by robot
* Collision probability by robot
* Collision avoidance possibility by robot

When configuring the integrated system, if risk factors are not sufficiently removed with the robot's safety-related functions (e.g., use of tools for non-collaborative robots, etc.), you should install necessary additional protective devices through risk assessment.
