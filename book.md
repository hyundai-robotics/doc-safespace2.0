
[__SOURCE](README.md)
# Hi7 Controller Function Manual - SafeSpace2.0

[__SOURCE](0-about-this-manual/README.md)
# About the Manual

[__SOURCE](0-about-this-manual/precautions.md)
# Precautions

{% include file="en/precautions.md" %}

[__SOURCE](0-about-this-manual/safety-notice.md)
# Safety Cautions

{% include file="en/safety-notice.md" %}

{% hint style="warning" %}
- Control through external communication commands and applications is not a safety function and shall not be used as a substitute for a safety-related control system.
- Safety functions such as SafeSpace and Soft Joint are supplementary risk-reduction measures and do not replace external safety fencing, interlocks, or risk assessments.
{% endhint %}

[__SOURCE](1-safety/README.md)
# 1. Safety


[__SOURCE](1-safety/1-safety-requirements/README.md)
# 1.1 Safety Requirements


[__SOURCE](1-safety/1-safety-requirements/1-applicable-standards.md)
# 1.1.1 Applicable Standards

This product has been designed and manufactured in accordance with the industrial robot safety standard ISO 10218-1 and the technical specification ISO/TS 15066 for collaborative operation. The safety standards applied to this product are as follows.

* ISO 10218-1:2025 Robots and robotic devices - Safety requirements for industrial robots - Part 1: Robots
* ISO 10218-2:2025 Robots and robotic devices - Safety requirements for industrial robots - Part 2: Robot systems and integration
* ISO/TS 15066:2016 Robots and robotic devices - Safety requirements - Industrial collaborative workspace
* IEC 61508-1:2010 Functional safety of electrical/electronic/programmable electronic safety-related systems - Part 1: General requirements
* IEC 61508-2:2010 Functional safety of electrical/electronic/programmable electronic safety-related systems - Part 2: Requirements for electrical/electronic/programmable electronic safety-related systems
* IEC 61508-3:2010 Functional safety of electrical/electronic/programmable electronic safety-related systems - Part 3: Software requirements
* IEC 61508-4:2010 Functional safety of electrical/electronic/programmable electronic safety-related systems - Part 4: Definitions and abbreviations
* IEC 61508-5:2010 Functional safety of electrical/electronic/programmable electronic safety-related systems - Part 5: Examples of methods for the determination of safety integrity levels
* IEC 61508-6:2010 Functional safety of electrical/electronic/programmable electronic safety-related systems - Part 6: Guidelines on the application of IEC 61508-2 and IEC 61508-3
* IEC 61508-7:2010 Functional safety of electrical/electronic/programmable electronic safety-related systems - Part 7: Overview of techniques and measures
* IEC 61800-5-1:2022 PRV Adjustable speed electrical power drive systems - Part 5-1: Safety requirements - Electrical, thermal and energy
* IEC 61800-5-2:2016 Adjustable speed electrical power drive systems - Part 2: General requirements - Rating specifications for low voltage adjustable speed a.c. power drive systems
* ISO 13849-1:2023 Safety of machinery - Safety-related parts of control systems - Part 1: General principles for design
* ISO 13849-2:2012 Safety of machinery - Safety-related parts of control systems - Part 2: Validation
* IEC 62061:2021 Safety of machinery. Functional safety of safety-related electrical, electronic and programmable electronic control systems
* IEC 61784-3:2016 Industrial communication networks - Profiles - Part 3: Functional safety fieldbuses - General rules and profile definitions
* IEC 61800-3:2022 Adjustable speed electrical power drive systems - Part 3: EMC requirements and specific test methods
* IEC 61000-6-7:2014 Electromagnetic compatibility (EMC) - Part 6-7: Generic standards - Immunity requirements for equipment intended to perform functions in a safety-related system (functional safety) in industrial locations
* IEC 61326-3-1:2017 Electrical equipment for measurement, control and laboratory use. EMC requirements. Part 3-1: Immunity requirements for safety-related systems and for equipment intended to perform safety-related functions (functional safety) - General industrial applications

[__SOURCE](1-safety/1-safety-requirements/2-safety-performance.md)
# 1.1.2 Safety Performance

![SafeSpace2.0 configuration](../../_assets/safety_diagram_en.png)


The safety performance of SafeSpace2.0's emergency stop and external device interface (basic safety input/output, PROFIsafe) is as follows:
|            **Item**            | **Safety Performance** |         **Applicable Standard**         |
| :--------------------------: | :-------: | :-----------------------: |
|              HFT             |     1     | IEC 61508/62061/61800-5-2 |
| SIL (Safety Integrity Level) |     3     | IEC 61508/62061/61800-5-2 |
|           Category           |     4     |        ISO 13849-1        |
|    PL (Performance Level)    |     e     |        ISO 13849-1        |
|    		PFH    			   |  1.5E-08  |         IEC 61508         |


The safety performance of other safety functions is as follows:
|            **Item**            | **Safety Performance** |         **Applicable Standard**         |
| :--------------------------: | :-------: | :-----------------------: |
|              HFT             |     1     | IEC 61508/62061/61800-5-2 |
| SIL (Safety Integrity Level) |     2     | IEC 61508/62061/61800-5-2 |
|           Category           |     3     |        ISO 13849-1        |
|    PL (Performance Level)    |     d     |        ISO 13849-1        |
|    		PFH    			   |  1.5E-07  |         IEC 61508         |



[__SOURCE](1-safety/2-safety-measures/README.md)
# 1.2 Safety Measures

Describes the safety functions built into the product and also the measures to ensure the safety of users and workers.

[__SOURCE](1-safety/2-safety-measures/1-safety-functions.md)
# 1.2.1 Safety functions

### Safety functions in SafeSpace2.0
SafeSpace2.0 is intended to carry out collaborative tasks based on the following safety functions. For the details of the safety functions, see the "[3. SafeSpace2.0 Safety functions](../../3-safety-function/README.md)"

* STO: Safe Torque Off
* SS1: Safe Stop 1
* SS2: Safe Stop 2
* Emergency Stop
* Protective Stop
* Normal Stop
* SOS: Safe Operating Stop
* Stopping time Monitoring
* Stopping distance Monitoring
* Joint-SLP, Joint Angle Monitoring
* Joint-SLS, Joint Angular Speed Monitoring
* TCP-SLP, TCP Position Monitoring
* TCP Orientation Monitoring
* TCP-SLS, TCP Speed Monitoring
* Power Monitoring
* Momentum Monitoring
* Collision Detection
* Speed and Separation Monitoring
* SBC: Safe Brake Control
* Safety Inputs
* Safety Outputs
* PROFIsafe
* Start/restart Interlock

---


### Option license
SafeSpace 2.0 is available with three different license options. Each license grants access to different functional specifications. For further details, please consult the table provided below. 

|  **Safety Functions** |                       **Default**                       |  **Option 1 (Basic)**  |  **Option 2 (Pro)**  |  **Option 3 (Collaborative)**  |
| :-------: | :------------------------------------------------: | :----------: | :----------: | :----------: |
| Emergency Stop/Protective Stop(SGG,SGA) |  O  | O | O | O |
| TCP speed monitoring in manual mode |  O  | O | O | O |
| Stopping distance/Stopping time monitoring |  O  | O | O | O |
| Joint position monitoring |    | O | O | O |
| TCP position monitoring |    | O | O | O |
| Position monitoring space |    | 1 | 16 | 16 |
| Joint speed monitoring |    |  | O | O |
| TCP speed monitoring |    |  | O | O |
| TCP orientation monitoring |    |  | O | O |
| Safe operating stop |    |  | O | O |
| Self collision monitoring |    |  | O | O |
| Speed and Separation monitoring |    |  |  | O |
| Collision/Power/Momentum monitoring |    |  |  | O |
| Safe motion |    |  |  | O |

[__SOURCE](1-safety/2-safety-measures/2-safety-training.md)
# 1.2.2 Safety Training

To effectively use the product's functions, you must familiarize yourself with the contents of the manual and properly install, use, and maintain the product. Product users have the responsibility to be familiar with and comply with robot-related safety regulations in the region where the robot is installed and used, and to properly design, install, and operate safety devices to ensure the safety of users working in the robot system.

* All workers who install, use, and maintain the robot system must thoroughly read the manual to fully understand its contents. In particular, be sure to familiarize yourself with the safety precautions (:warning:).
* We plan and implement trainings related to the installation, use, and maintenance of the product. Product users and workers must complete the corresponding training course before using the product.
* Workers responsible for teaching and inspecting the robot must complete trainings for robot use and safety before using the robot. The safety training program covers the following:
  * Safety concepts, and the purpose and functions of safety devices
  * Procedures for safely handling the robot
  * Performance and potential risk factors of the robot and robot system
  * Work related to specific applications of the robot, etc.

[__SOURCE](1-safety/2-safety-measures/4-emergency-stop/README.md)
# 1.2.3 Emergency Stop

The emergency stop function operates in emergencies or emergency situations such as when a worker or other object enters a danger area. All emergency stop switches are installed in locations that are easily accessible even from outside the safety area.

When the emergency stop function is executed, the robot immediately stops the operation in any case.

* The robot servo system power is cut off and the motor brake operates.
* The teach pendant screen displays an emergency stop message.

[__SOURCE](1-safety/2-safety-measures/4-emergency-stop/1-switches.md)
# 1.2.3.1 Emergency Stop Switch

There is one emergency stop switch installed on the controller and one on the teach pendant. Press the emergency stop switch in case of an emergency.

[__SOURCE](1-safety/2-safety-measures/4-emergency-stop/2-connecting-to-devices-of-external-system.md)
# 1.2.3.2 Connecting External Emergency Stop Device

In addition to the pre-installed emergency stop switch, an external emergency stop device can be connected depending on the field environment and application. For more information, see "[2. Installation](../../../2-installation/README.md)" and "[3.3.4 Safety Signal Input/Output](../../../3-safety-function/3-safety-function/4-safety-io/README.md)".


[__SOURCE](1-safety/3-risk-assessment.md)
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

[__SOURCE](1-safety/4-potential-risks.md)
# 1.4 Potential Hazards

If the risk assessment of the integrated system linked with the robot concludes that risk factors are not sufficiently removed with the robot's safety-related functions alone, you must establish additional protective measures.

Matters to consider when establishing additional protective measures are as follows:

* Finger caught-in/between (entrapment) between the robot base and installation base during installation
* Injuries (stabbing, penetration, etc.) caused by sharp edges or pointed parts of obstacles or tools in the work area.
* Injuries (bruising, falling, fracture, etc.) from collision with the robot
* Injuries (stabbing, penetration, fracture, etc.) caused by obstacles around the robot
* Injuries that may occur when fastening parts are not completely fixed
* Injuries that may occur when working with toxic or harmful substances (skin damage, difficulty breathing, etc.)
* Workpiece separation from the tool due to sudden power interruption
* Mistakes that may occur due to confusion with the emergency stop switches of other equipment
* Errors due to unauthorized changes to safety-related function settings, etc.

The types of possible hazards vary depending on the system configuration, so you must conduct a risk assessment before using the integrated system.

[__SOURCE](1-safety/5-validity-and-responsibilities.md)
# 1.5 Validity and Responsibility

It is required to comply with the safety requirements based on the safety regulations and laws of the country and region where the robot is installed and used. The supplier and user of the integrated robot system have various responsibilities including the following:

* Risk assessment of the integrated robot system
* Addition and removal of safety devices according to risk assessment results
* Verification of proper configuration, installation, and setting of the integrated system
* Establishment of methods and guidelines for using the integrated system and user training
* Management of safety devices (prohibition of unauthorized changes and manipulation of safety devices by users)
* Provision of information such as critical information of the product use and safety, and also the contact information, etc.
* Provision of all types of technical documents including manuals, etc.

The safety-related content in this manual does not cover all possible risk factors and situations that may occur while using the product.

[__SOURCE](1-safety/6-reaction-time.md)
# 1.6 Response Time


* **Stop Response Time**

The response time to be taken from safety function violation to stop execution is 9.8ms. The response time should be reflected when calculating the robot's stop time and stop distance.


* **Safety Input Response Time (Safety Input)**

The maximum response time from the receipt of a stop signal through a safety input (**Default** or **Additional**) until the stop action is initiated is **11 ms**. This value does not include the input signal filter time, nor does it include the robot stopping time or stopping distance.

* **Safety Input Response Time (Safety Communication)**

The maximum response time from the receipt of a stop signal through safety communication until the stop action is initiated is **42 ms**. To obtain the total time required for the robot to come to a complete stop, the safety communication cycle time and the robot stopping time and stopping distance shall be taken into account.

* **Safety Output Response Time (Safety Communication)**

The maximum response time from the generation of a safety output by the safety application until the signal is transmitted through safety communication is **28 ms**. To calculate the total transmission time to the safety PLC, the safety communication cycle time shall be added.



[__SOURCE](2-installation/README.md)
# 2. Installation


[__SOURCE](2-installation/1-robot-system.md)
# 2.1 Robot System

An industrial robot is a machine equipped with automatic control, manipulation, and movement functions, capable of executing various tasks programmed in industrial settings. Collaborative robots are a type of industrial robot.

A robot system consists of a robot body and a controller that controls the body. A teach pendant is attached to the controller, which allows for setup and manual operation of the robot system.

* Robots: Perform various tasks in industrial settings, such as transporting objects or assembling parts.
* Controller: Coordinates the robot's movements according to program settings set via the teach pendant. The controller's input/output ports can be used to interface with various external equipment or devices.
* Teach Pendant: This device manages the entire robot system. It can be used to teach the robot specific postures or to set and control programs.

Examples of basic robot system configurations, depending on the robot type, are as follows:


![Basic configuration of a vertical multi-joint robot system](../_assets/image_7.png)

{% hint style="info" %}
For more information about the robot system, please refer to the "[Hi7 Controller Operating Instructions](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/en-tp630/1-robot-system/README?cont_model=Hi7)".
{% endhint %}

[__SOURCE](2-installation/2-scm-install.md)
# 2.2 Safety Module

The safety control module is shipped mounted inside the controller in board form. When board replacement is required, refer to the controller maintenance manual.
[__SOURCE](2-installation/3-add-io-install.md)
# 2.3 I/O Module (Option)

When you select to use the I/O option module, it is shipped mounted inside the controller. When board replacement is required, refer to the controller maintenance manual.
[__SOURCE](2-installation/4-profisafe-install.md)
# 2.4 PROFIsafe Module (Option)

When you select to use the PROFIsafe option module, it is shipped mounted inside the controller. When board replacement is required, refer to the controller maintenance manual.
[__SOURCE](3-safety-function/README.md)
# 3. SafeSpace2.0 Safety Functions


[__SOURCE](3-safety-function/1-description-term.md)
# 3.1 Terminology

### <mark style="color:green;">Robot Monitoring Function</mark>&#xD;

Parameters that serve as the references for monitoring the robot's speed, force, and momentum.

* **Joint Angle Monitoring**

Monitors the position of each axis joint. Performs a user-set safety stop if the reference value is exceeded.

* **Joint Speed Monitoring**

Monitors the speed of each axis joint. Performs a user-set safety stop if the reference value is exceeded.
    
* **Safe Operating Stop (SOS) Monitoring**

Monitors whether each axis maintains a stopped state without slip. Performs Stop 0 if the reference value is exceeded.

* **TCP Position Monitoring**

Monitors whether the safety tool model violates the safety area. Performs a user-set safety stop if the area is violated.
    
* **TCP Orientation Monitoring**

Monitors whether the tool orientation stays within the specified range. Performs a user-set safety stop if the reference value is exceeded.
    
* **TCP Speed Monitoring**

Monitors the speed of the TCP. Performs a user-set safety stop if the reference value is exceeded.
    
* **Power Monitoring**

Monitors the robot's power. Performs a user-set safety stop if the reference value is exceeded.
    
* **Momentum Monitoring**

Monitors the robot's momentum. Performs a user-set safety stop if the reference value is exceeded.


* **Collision Detection**

Performs a user-set safety stop when an external force applied to the robot exceeds the allowable value.


### <mark style="color:green;">Safety Layout</mark>

Parameters for the safety areas and tool areas that serve as the references for the monitoring of the TCP position and orientation.

* **Safety Area**

General term for the tool's work area and protected area
* **Work area**

The area where the robot performs work. Performs a safety stop if the tool model and robot elbow model leave the work area.
* **Protected Area**

The area that should be protected from the robot. Performs a safety stop if the tool model and robot elbow model violate the protected area.
* **Safety Tool Modeling**

Models the tool attached to the robot as a sphere and cone for the TCP position and orientation monitoring
* **Safety Robot Modeling**

Models the robot's 2nd and 3rd axes as capsules to monitor the distance from the safety area



### <mark style="color:green;">Safety Stop</mark>&#xD;

Stops the robot to create a safe state when safety is violated. There are 3 stop methods. For detailed information on each stop method, refer to "ISO 13850" or "IEC 60204-1."

* **Stop 0**

Immediately removes the power from the motor of each join and stop the joints (uncontrolled stop).
* **Stop 1**

Motors of all joints decelerate and stop, then power is removed from the motors (controlled stop). The robot decelerates to a stop while continuously following the program path and the power is cut off as soon as the robot stops.
* **Stop 2**

The motor of each joint decelerates and then Safe Operating Stop (SOS) monitoring operates. Power supply to all motors is maintained.


Stop 1 and Stop 2 functions monitor the deceleration process through deceleration time and distance.

* **Stop Time**

Monitors the time from the start of deceleration to the actual stop. If the robot does not stop within the set time, Stop 0 is performed to immediately remove the power from the motors.
* **Stop Distance**

Monitors the TCP distance from the start of deceleration to the actual stop. If the robot does not stop within the set distance, Stop 0 is performed to immediately remove the power from the motors.



### <mark style="color:green;">Safe Motion Tuning</mark>&#xD;

This function automatically adjusts robot motion to avoid exceeding the entered parameters.
The following parameters are considered during motion tuning:

* **Joint Speed**

* **TCP Speed**

* **Power**

* **Momentum**

* **Stopping Time**

* **Stopping Distance**
[__SOURCE](3-safety-function/2-limitations.md)
# 3.2 Limitations

SafeSafe2.0 has the following limitations. Please check their applicability before configuring the feature.


|  **Item** |                       **Description**                      |
| :-------: | :------------------------------------------------: |
| Supported Robots | 6-axis Industrial Robots, Collaborative Robots |
| Unsupported Robots | FPD Robots, Painting Robots, Gantry Robots | 
| Supported Axes | Up to 8 axes (For systems with 9 or more axes, safety functions can only be configured for axes 7 and 8) |
| Unsupported Robot Axes | Servogun Axes, Additional Axes Combined with Robots (Gantry Robots) |
[__SOURCE](3-safety-function/3-safety-function/README.md)
# 3.3 Safety Functions


SafeSpace2.0 safety functions can be configured through safety function settings and are used as risk countermeasures selected in the risk assessment performed by the worker.


[__SOURCE](3-safety-function/3-safety-function/1-general-condition/README.md)
# 3.3.1 General Setup

Robot safety parameters consist of limit values   and stop methods for monitoring safety functions.

Each safety function can be configured with various activation conditions, stop methods upon violation, and limit values.

Access the safety function basic settings menu using the following methods.

* `[System > 10: Safety System > 1: General setup]`
****

The following safety functions can be configured in the Basic Settings menu:

* **General**: Set safety function activation, manual mode speed, stopping distance, and periodic time monitoring.
* **Stop Settings**: Set the stopping method (Stop 0, Stop 1, Stop 2) according to the stop type.
* **Safety Tool Information**: Set safety tool information.
* **Safety Added Weight**: Set the safety added weight.
* **Maintenance**: Set the robot test cycle required for safety function maintenance.

{% hint style="warning" %}
<strong>[Caution]</strong>: Operators and users must perform a risk assessment before configuring robot safety functions to ensure the safety of personnel and equipment surrounding the robot. Based on the assessment results, configure the following:

* Set a password, etc. to prevent unauthorized changes to the safety configuration.
* Configure safety-related functions and interfaces.
* Verify the accuracy of settings before operating the robot.
* Verify that all safety function configurations and settings comply with the risk assessment.
{% endhint %}


[__SOURCE](3-safety-function/3-safety-function/1-general-condition/1-general.md)
# 3.3.1.1 General

Set the thresholds for essential functions (manual mode speed monitoring, stop time, and stop distance monitoring) required for robot operation. Additionally, configure whether the robot monitoring and area monitoring functions are fully enabled. Even if the robot monitoring and area monitoring functions are enabled, if the safety function is disabled, the monitoring function will not operate. If a monitoring violation occurs, the configured safety stop (Stop 0, Stop 1) will be immediately activated.


You can set parameter values in the `[System > 10: Safety System > 1: General setup > 1: General]` menu.

<p align="center">
<img src="../../../_assets/3/general.png"></img>
<em><p align="center">General parameter setting screen</p></em>
</p>


|  **Parameter** |                       **Description**                       |  **Default setting**  |
| :-------: | :------------------------------------------------: | :-------------: |
| Safety function | <p>Whether robot monitoring and area monitoring functions are enabled</p><p>(Enable / Disable)</p> | Disable |
| <p>Manual mode speed</p><p>[mm/s]</p> | <p>Whether the function is enabled</p><p>(10 ~ 250)</p> | 250 |
| <p>Stop time</p><p>[ms]</p> | <p>Stop method when the function is violated</p><p>(100 ~ 2000)</p> | 2000 |
| - Motion Tuning | <p>Tuning to a motion that satisfies the stopping time limit</p><p>(Enable / Disable)</p> | Disable |
| <p>Stopping Distance</p><p>[mm]</p> | <p>Whether each joint is activated</p><p>(50 ~ 2000)</p> | 2000 |
| - Motion Tuning | <p>Tuning to a motion that satisfies the stopping distance limit</p><p>(Enable / Disable)</p> | Disable |

{% hint style="warning" %}
<strong>[Caution]</strong>: Even if the safety function is set to disabled, the functions that are essential for robot use (manual mode speed, stop time, stop distance monitoring) are not disabled.
{% endhint %}

{% hint style="warning" %}
<strong>[Caution]</strong>: The stop time and stop distance are the time and distance until the robot actually stops when stop1 is executed, and if the set value is exceeded, stop0 is activated immediately.
{% endhint %}
 
[__SOURCE](3-safety-function/3-safety-function/1-general-condition/2-safe-stop.md)
# 3.3.1.2 Stop Settings

Set the appropriate safe stop type for each safety function. Safe stop functions stop the robot to a safe state when a safety violation occurs. There are three types: All types of safe stop functions comply with Requirement 4.2.2.4 of IEC 61800-5-2.


* **Stop 0**: Immediately remove power from all motors in the joint modules and stop.
* **Stop 1**: All motors in the joint modules decelerate and then stop. Power is then removed from the motors.
* **Stop 2**: All motors in the joint modules decelerate and SOS (Safe Operating Stop) is activated. Power is maintained to all motors.


The stop type due to a safety function violation is set in the function-specific parameter setting menu.
You can set the stop method according to the stop type (emergency stop, protective stop, normal stop) required by ISO 10218-1.
For signal inputs for each stop, refer to "[3.3.4 Safety Signal Input/Output](../../../3-safety-function/3-safety-function/4-safety-io/README.md)."
You can also set the stop method to be performed when the manual mode speed monitoring is violated. The stop method can be selected from Stop 0 or Stop 1.

You can set the parameter values in the `[System > 10: Safety System > 1: General setup > 2: Safe Stop]` menu.

<p align="center">
<img src="../../../_assets/3/safety_stop.png"></img>
<em><p align="center">Stop parameter setting screen</p></em>
</p>


|  **Parameter** |                       **Description**                       |  **Default value**  |
| :-------: | :------------------------------------------------: | :-------------: |
| Emergency stop | <p>Select the stop type to apply in case of emergency stop</p><p>(Stop 0, Stop 1)</p> | Stop 1 |
| Protective stop | <p>Select the stop type to apply in case of protective stop</p><p>(Stop 0, Stop 1, Stop 2)</p> | Stop 1 |
| Normal stop | <p>Select the stop type to apply in case of normal stop</p><p>(Stop 0, Stop 1)</p> | Stop 1 |
| Manual stop | <p>Select the stop type to apply in case of manual mode stop</p><p>(Stop 0, Stop 1)</p> | Stop 1 |

{% hint style="warning" %}
<strong>[Caution]</strong>: Appropriate stopping methods for each function must be established through risk assessment, and verification must be performed before operation. 
{% endhint %}
 
[__SOURCE](3-safety-function/3-safety-function/1-general-condition/3-safe-tool-info.md)
# 3.3.1.3 Safety Tool Information

Safety tool information is used by the safety board to calculate the robot's speed and position. You must enter the tool information attached to the actual robot. The tool information must be identical to the tool number used for robot control `[System > 3: Robot Parameters > 1: Tool Data]`.


You can set safety tool information in the `[System > 10: Safety System > 1: General setup > 3: Safety Tool Information]` menu. After setting the robot tool number, you can load tool information used for robot control by clicking [Load Tool Data] at the bottom of the menu.

<p align="center">
<img src="../../../_assets/3/tool_info.png"></img>
<em><p align="center">Safety tool parameter setting screen</p></em>
</p>


|  **Parameter** |                       **Description**                       |  **Default value**  |
| :-------: | :------------------------------------------------: | :-------------: |
| <p>Robot tool number</p> | <p>Tool number used by the robot. A value of -1 indicates that it is not used.</p><p>(-1 ~ 31)</p> | -1 |
| <p>Weight</p><p>[kg]</p> | <p>Weight of the tool</p><p>(0.0 ~ 1000.0)</p> | 0.0 |
| <p>Length</p><p>[mm]</p> | <p>Length of the tool</p><p>(-3000.0 ~ 3000.0)</p> | 0.0 |
| <p>Center</p><p>[mm]</p> | <p>Location of the center of gravity of the tool relative to the center of the flange</p><p>(-3000.0 ~ 3000.0)</p> | 0.0 |
| <p>Inertia</p><p>[kg·㎡]</p> | <p>Moment of inertia of the tool with respect to the tool coordinates</p><p>(0.0 ~ 2000.000)</p> | 0.0 |
| Load Tool Data | A function to load tool information used for robot control according to the tool number | - |
| Copy | A function to copy the values   entered on the corresponding page | - |
| Paste | A function to paste the values   of the copied page onto the corresponding page | - |

{% hint style="warning" %}
<strong>[Caution]</strong>: If the safety tool information does not match the tool information used for robot control, a warning/error will occur and the robot will not operate. Be sure to match the actual tool information with the safety tool information before operating the robot.
{% endhint %}
[__SOURCE](3-safety-function/3-safety-function/1-general-condition/4-safe-additional-load.md)
# 3.3.1.4 Safety Added Weight

Safety added weight information is used by the safety board to calculate the robot's torque. You must enter the information for the added weight actually installed on the robot. The information must be identical to the added weight information used for robot control `[System > 3: Robot Parameter > 7: Additional Weight on Each Axis]`.


* `[System > 10: Safety System > 1: General setup > 4: Safety Additional Load]` You can set the safety additional weight information in the menu, and you can load the additional weight information used for robot control by clicking "Load Additional Weights" at the bottom of the menu.


<p align="center">
<img src="../../../_assets/3/add_tool.png"></img>
<em><p align="center">Safety Added weight parameter setting screen</p></em>
</p>


|  **Parameter** |                       **Description**                       |  **Default value**  |
| :-------: | :------------------------------------------------: | :-------------: |
| <p>Weight</p><p>[kg]</p> | <p>Weight of the tool</p><p>(0.0 ~ 1000.0)</p> | 0.0 |
| <p>Center</p><p>[mm]</p> | <p>Position of the center of gravity of the tool relative to the center of the flange</p><p>(-3000.0 ~ 3000.0)</p> | 0.0 |
| <p>Inertia</p><p>[kg·㎡]</p> | <p>Moment of inertia of the tool with respect to the tool coordinates</p><p>(0.0 ~ 2000.000)</p> | 0.0 |
| Load add Weights | A function to load additional weight information used for robot control | - |
| Copy | A function to copy the values   entered on the corresponding page | - |
| Paste | A function to paste the values   from the copied page onto the corresponding page | - |

{% hint style="warning" %}
<strong>[Caution]</strong>: If the safety weight information and the weight information used for robot control do not match, a warning/error will occur and the robot will not be able to operate. Be sure to match the weight information with the actual attached weight before operating the robot. 
{% endhint %}
 
{% hint style="warning" %}
<strong>[Caution]</strong>: The safety additional weight number is supported from 0 to 2, and each number matches the axis number of the system additional weight (0-S axis, 1-H axis, 2-V axis). Please enter the additional weight information by matching the safety parameter number with the axis number.
{% endhint %}
 
 
[__SOURCE](3-safety-function/3-safety-function/2-robot-safety-condition/README.md)
# 3.3.2 Robot Monitoring Function

Robot safety parameters consist of limit values   and stop methods for monitoring safety functions.

Each safety function can be configured with various activation conditions, stop methods upon violation, and limit values.

To configure robot safety parameters, access the menu as follows:

* `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction]`
****

The following safety features can be configured in the Robot Limits menu:

* **Joint Space**: Limits the robot's range of motion for each axis to a specific range.
* **Joint Speed**: Limits the robot's motion by preventing it from exceeding the speed limit for each axis.
* **Joint Stop**: Monitors the robot's stopped state by checking for abnormal movement for each axis after performing Stop 2.
* **TCP Speed**: Limits the robot's speed to a specified speed based on TCP standards.
* **Collision Detection**: Limits the force in the event of a collision between the robot and the worker.
* **RePlan**: Adjusts the robot's speed according to external input to perform "3.2.2 "Speed and Position Monitoring" during collaborative operation mode.
* **Power Detection**: Limits the force in the event of a collision between the robot and the worker.
* **Momentum**: Limits the energy and impact load in the event of a collision between the robot and the worker.

{% hint style="warning" %}
**\[Caution]** : When the speed limit of any of the following safety functions is changed, it may take up to 10 ms for the new limit to become effective. In addition, for the Replan function, extra deceleration time may be required depending on the current operating conditions until the robot complies with the updated speed limit. This behavior shall be taken into consideration.
* Joint Speed Limit 
* TCP Speed Limit 
* Replan
{% endhint %}

{% hint style="warning" %}
<strong>[Caution]</strong>: Operators and users must perform a risk assessment before configuring robot safety functions to ensure the safety of personnel and equipment surrounding the robot. Based on the assessment results, configure the following:

* Set a password, etc. to prevent unauthorized changes to the safety configuration.
* Configure safety-related functions and interfaces.
* Verify the accuracy of settings before operating the robot.
* Verify that all safety function configurations and settings comply with the risk assessment.
{% endhint %}


[__SOURCE](3-safety-function/3-safety-function/2-robot-safety-condition/1-joint-space.md)
# 3.3.2.1 Joint Space Setting

The Joint space Setting parameter is a limit value for monitoring safety functions in the robot's joint space. If the monitoring is violated, the specified safety stop (Stop 0, Stop 1, or Stop 2) is immediately activated.

<p align="center">
<img src="../../../_assets/joint_space.PNG"></img>
<em><p align="center">Joint space setting example (S-axis)</p></em>
</p>

You can set parameter values in the `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 1: Joint space]` menu.

<p align="center">
<img src="../../../_assets/3/joint_space.png"></img>
<em><p align="center">Joint space parameter setting screen</p></em>
</p>


|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Type | <p>Safety Area Type</p><p>(Working Area / Protection Area)</p> | Working Area |
| Activation | <p>Whether the function is activated</p><p>(OFF / ON / Safety I/O)</p> | OFF |
| Stop function | <p>Stop method in case of function violation</p><p>(Stop 0 / Stop 1 / Stop 2 / No Stop)</p> | Stop 1 |
| Joint ON/OFF | <p>Whether each joint is activated</p><p>(OFF / ON)</p> | OFF |
| <p>Minimum</p><p>[deg]</p> | <p>Minimum limits for each joint angle</p><p>(-360.0 ~ 360.0)</p> | -360.0 |
| <p>Maximum</p><p>[deg]</p> | <p>Maximum limits for each joint angle</p><p>(-360.0 ~ 360.0)</p> | 360.0 |

{% hint style="warning" %}
<strong>[Caution]</strong>: The safety function monitors based on the set area. The set area should be configured considering the stop distance, and verification must be performed before operation.
{% endhint %}
 
[__SOURCE](3-safety-function/3-safety-function/2-robot-safety-condition/2-joint-speed.md)
# 3.3.2.2 Joint Speed Limit

The Joint Speed Setting parameter is a limit value for monitoring the robot's joint speed. If the limit value is violated, the specified safety stop (Stop 0, Stop 1, or Stop 2) is immediately activated.

<p align="center">
<img src="../../../_assets/joint_speed.PNG"></img>
<em><p align="center">Joint speed setting example</p></em>
</p>

You can set parameter values   in the `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 2: Joint speed]` menu.

<p align="center">
<img src="../../../_assets/3/joint_speed_set.png"></img>
<em><p align="center">Joint speed setting parameter setting screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Whether the function is activated</p><p>(OFF / ON / Safety I/O)</p> | OFF |
| Stop function | <p>Stop method when the function is violated</p><p>(Stop 0 / Stop 1 / Stop 2 / No stop)</p> | Stop 1 |
| Motion Tuning | <p>Tuning to a motion that does not exceed the joint's speed limit</p><p>(Active / Disable)</p> | Disable |
| Joint ON/OFF | <p>Whether each joint is activated</p><p>(ON / OFF)</p> | OFF |
| <p>Speed</p><p>[mm/s]</p> | <p>Speed limit for each joint</p><p>(10 ~ 10000)</p> | 1000.0 |

{% hint style="warning" %}
<strong>[Caution]</strong>: When setting the speed monitoring function, be sure to consider the stopping reaction time and cover the cover to prevent collisions and injuries.
{% endhint %}
 

[__SOURCE](3-safety-function/3-safety-function/2-robot-safety-condition/3-joint-SOS.md)
# 3.3.2.3 Joint Stop Monitoring

Stop monitoring monitors each axis for abnormal movement during robot stop operations. If a set limit is violated, a safety stop (Stop 0) is immediately activated.

Parameter values   can be set in the `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 3: Joint SOS]` menu.

<p align="center">
<img src="../../../_assets/3/joint_sos.png"></img>
<em><p align="center">Stop Monitoring Parameter Setting Screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Whether the function is activated</p><p>(OFF / ON / Safety I/O)</p> | OFF |
| Joint ON/OFF | <p>Whether each joint is activated</p><p>(ON / OFF)</p> | OFF |
| <p>Tolerance</p><p>[deg]</p> | <p>Angle Limit Value for Each Joint</p><p>(0.0 ~ 3.0)</p> | 0.100 |

{% hint style="warning" %}
<strong>[Caution]</strong>: If the stop monitoring parameters are violated, be sure to check that the robot's movement is normal before restarting.
{% endhint %}
[__SOURCE](3-safety-function/3-safety-function/2-robot-safety-condition/4-tcp-speed.md)
# 3.3.2.4 TCP Speed Limit Setting

This function monitors the TCP speed relative to the robot coordinate system. If a monitoring violation occurs, a safety stop (Stop 0, Stop 1, or Stop 2) is immediately activated.

You can set the parameter values   in the `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 4: TCP Speed]` menu.

<p align="center">
<img src="../../../_assets/3/tcp_speed.png"></img>
<em><p align="center">TCP speed parameter setting screen</p></em>
</p>


| **Parameter** |                                  **Description**                                  |  **Default Setting** |
| :------: | :----------------------------------------------------------------: | :---------: |
| Activation | <p>Whether the function is activated</p><p>(OFF / ON / Safety I/O)</p> | OFF |
| Stop function | <p>Stop method in case of function violation</p><p>(Stop 0 / Stop 1 / Stop 2 / No stop)</p> | Stop 1 |
| Motion tuning | <p>Tuning to a motion that does not exceed the TCP speed limit</p><p>(Enable / Disable)</p> | Disable |
| <p>Limit</p><p>[mm/s]</p> | <p>TCP speed limit value</p><p>(1 ~ 50000)</p> | 50000 |

{% hint style="warning" %}
<strong>[Caution]</strong>: When setting the speed monitoring function, be sure to consider the stopping reaction time and cover the cover to prevent collisions and injuries.
{% endhint %}
 
[__SOURCE](3-safety-function/3-safety-function/2-robot-safety-condition/5-collision.md)
# 3.3.2.5 Collision Detection

When the external force applied to the robot exceeds the allowable value, it is recognized as a collision. You can adjust the sensitivity of each axis, and the higher the sensitivity, the more even a small external force is recognized as a collision. When the monitoring is violated, a safety stop (Stop 0, Stop 1, and Stop 2) is immediately activated.

`[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 5: Collision detection]` menu allows you to set the parameter values.

<p align="center">
<img src="../../../_assets/3/collision.png"></img>
<em><p align="center">Collision detection parameter setting screen</p></em>
</p>

| **Parameter** |                                  **Description**                                  |  **Default Setting** |
| :------: | :----------------------------------------------------------------: | :---------: |
| Activation | <p>Function activation status</p><p>(OFF / ON / Safety Input / Hand Guiding Control)</p> |   OFF  |
| Stop function |   <p>Stop method when the function is violated</p><p>(Stop 0, Stop 1, Stop 2, Non-stop)</p>  | Stop 1 |
| Joint ON/OFF |   <p>Activation status of each joint</p><p>(ON/OFF)</p>  |  OFF |
| Sensitivity |   <p>Detection sensitivity for each joint</p><p>(1 ~ 200(%))</p>  |  100 |

{% hint style="warning" %}
<strong>[Caution]</strong> Since the robot's impact force can increase in proportion to kinetic energy when the speed is high and the payload is large, considerable impact may occur if the robot collides with an external object. In the collaborative space, operate while maintaining the safe speed and payload.
<strong>[Caution]</strong> False detection may occur if the tool information and additional weight are set differently from actual values. Check each information before using the collision detection function.
{% endhint %}

[__SOURCE](3-safety-function/3-safety-function/2-robot-safety-condition/6-re-plan.md)
# 3.3.2.6 Re plan Setting

Re plan is a function that adjusts the robot's speed based on signals received from external safety sensors. The robot's operating speed is adjusted to the deceleration rate corresponding to the input signal, and the TCP speed is monitored at the corresponding speed after a delay time.

If the delay time is insufficient or the robot decelerates insufficiently, resulting in a violation of the TCP speed limit, a safety stop (Stop 0) is immediately activated.

You can set the parameter values   in the `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 6: Re plan]` menu.

<p align="center">
<img src="../../../_assets/3/replan_param.png"></img>
<em><p align="center">Re plan settings screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Re plan | <p>Whether to use the speed control function according to the input signal</p><p>(Enable / Disable)</p> | Disable |
| <p>Delay time</p><p>[ms]</p> | <p>When changing the speed with Re plan, monitor the changed speed limit value after the delay time </p><p>(0 ~ 2000)</p> | 2000 |
| <p>Speed limit value</p><p>[mm/s]</p> | <p>TCP speed limit value after Re plan</p><p>(0 ~ 50000)</p> | 50000 |
| <p>Speed ratio</p><p>[%]</p> | <p>Deceleration ratio to use when Re plan</p><p>(0 ~ 100)</p> | 100 |
| <p>Input signal</p><p>[Type, Number]</p> | <p>Input signal for Re plan</p><p>( [None, -] / [default input, 3] / [additional input, 0~7] / [safety input, 0~63])</p> | 0 |

{% hint style="warning" %}
<strong>[Caution]</strong> When configuring speed limits, always consider stopping time and cover the robot to prevent collisions and injuries.
<strong>[Caution]</strong> High speeds and large payloads, in proportion to the robot's kinetic energy, can increase the robot's impact force. Therefore, a significant impact can occur if the robot collides with an external object. Maintain a safe speed and payload in collaborative spaces.
{% endhint %}

[__SOURCE](3-safety-function/3-safety-function/2-robot-safety-condition/7-power.md)
# 3.3.2.7 Power Setting

This function monitors whether the force generated by the robot exceeds the allowable limit. If a monitoring violation occurs, a safety stop (Stop 0, Stop 1, or Stop 2) is immediately activated.

You can set the parameter values   in the `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 7: Power]` menu.

<p align="center">
<img src="../../../_assets/3/power.png"></img>
<em><p align="center">Power settings screen</p></em>
</p>

| **Parameter** |          **Description**                                                  |  **Default Setting** |
| :------: | :----------------------------------------------------------------: | :---------: |
| Activation | <p>Whether the function is activated</p><p>(OFF / ON / Safety I/O / Hand Guiding Control)</p> | OFF |
| Stop function | <p>Stop method in case of function violation</p><p>(Stop 0 / Stop 1 / Stop 2 / No stop)</p> | Stop 1 |
| Motion tuning | <p>Tuning to a motion that does not exceed the robot's power limit</p><p>(Active / Disable)</p> | Disable |
| <p>Max power</p><p>[w]</p> | <p>Robot's power limit</p><p>(80 ~ 50000)</p> | 1000 |

{% hint style="warning" %}
<strong>[Caution]</strong> High speeds and large payloads, proportional to the robot's kinetic energy, can increase the robot's impact force. Therefore, a collision with an external object can result in significant impact. In collaborative spaces, maintain a safe speed and payload.
<strong>[Caution]</strong> Setting tool information and additional weights differently from actual values   may result in false detection. Please check the information before using this feature.
{% endhint %}

[__SOURCE](3-safety-function/3-safety-function/2-robot-safety-condition/8-momentum.md)
# 3.3.2.8 Momentum Setting

This function monitors whether the momentum generated by the robot exceeds the allowable limit. If a monitoring violation occurs, a safety stop (Stop 0, Stop 1, or Stop 2) is immediately activated.

You can set the parameter values   in the `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 8: Momentum]` menu.

<p align="center">
<img src="../../../_assets/3/momentum.png"></img>
<em><p align="center">Momentum settings screen</p></em>
</p>

| **Parameter** |          **Description**                                                  |  **Default Setting** |
| :------: | :----------------------------------------------------------------: | :---------: |
| Activation | <p>Whether the function is activated</p><p>(OFF / ON / Safety I/O / Hand Guiding Control)</p> | OFF |
| Stop function | <p>Stop method in case of function violation</p><p>(Stop 0 / Stop 1 / Stop 2 / No stop)</p> | Stop 1 |
| Motion tuning | <p>Tuning to a motion that does not exceed the robot's momentum limit</p><p>(Enable / Disable)</p> | Disable |
| <p>Max momentum</p><p>[kg m/s]</p> | <p>Robot's momentum limit</p><p>(5 ~ 50000)</p> | 1000 |

{% hint style="warning" %}
<strong>[Caution]</strong> High speeds and large payloads, proportional to the robot's kinetic energy, can increase the robot's impact force. Therefore, a collision with an external object can result in significant impact. In collaborative spaces, maintain a safe speed and payload.
<strong>[Caution]</strong> Setting tool information and additional weights differently from actual values may result in false detection. Please check the information before using this feature.
{% endhint %}

[__SOURCE](3-safety-function/3-safety-function/3-safety-layout/README.md)
# 3.3.3 Space Monitoring Function

Model the robot, tool, and safety zone to monitor the robot's position and orientation.

[__SOURCE](3-safety-function/3-safety-function/3-safety-layout/1-cell-area.md)
# 3.3.3.1 Safety Space Setting

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
| <p>Z Min / Max</p><p>[mm]</p> | <p>Height of the safe area based on the robot coordinate system</p><p>(-30000.0 ~ 30000.0)</p> | 0 |
| Enable | <p>Whether to enable the vertex of the safe area</p><p>(Enable / Disable)</p> | Disable |
| <p>X</p><p>[mm]</p> | <p>X-direction position of the vertex based on the robot coordinate system</p><p>(-30000.0 ~ 30000.0)</p> | 0 |
| <p>Y</p><p>[mm]</p> | <p>Y-direction position of the vertex based on the robot coordinate system</p><p>(-30000.0 ~ 30000.0)</p> | 0 |



{% hint style="warning" %}
**\[Caution]**: The safety function monitors based on the set area. The set area should be configured considering the stop distance, and verification must be performed before operation.
{% endhint %}
[__SOURCE](3-safety-function/3-safety-function/3-safety-layout/2-safety-tool-modeling.md)
# 3.3.3.2 Safety Tool Modeling

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

You can set parameter values   in the `[System > 10: Safety System > 2: Parameter setup > 2: Space restriction > 3: Tool]` menu.

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
| <p>X</p><p>[mm]</p> | <p>Model center position in X direction</p><p>(-3000.0 ~ 3000.0)</p> | 0 |
| <p>Y</p><p>[mm]</p> | <p>Model center position in Y direction</p><p>(-3000.0 ~ 3000.0)</p> | 0 |
| <p>Z</p><p>[mm]</p> | <p>Model center position in Z direction</p><p>(-3000.0 ~ 3000.0)</p> | 0 |
| <p>Rot.X</p><p>[deg]</p> | <p>X direction in flange coordinate system</p><p>(-180.0 ~ 180.0)</p> | 0 |
| <p>Rot.Y</p><p>[deg]</p> | <p>Y direction in flange coordinate system</p><p>(-180.0 ~ 180.0)</p> | 0 |
| <p>Rot.Z</p><p>[deg]</p> | <p>Z direction in flange coordinate system</p><p>(-180.0 ~ 180.0)</p> | 0 |





{% hint style="warning" %}
**\[Caution]**

* When changing tool data, be sure to recheck that the parameters set in safety tool modeling are accurate. The tool data number and safety tool modeling number of the same tool should match.
* As the definition of robot layout settings applies only to the robot 2nd and 3rd axes, other parts of the robot may violate this area even if a safety area is set.
{% endhint %}

[__SOURCE](3-safety-function/3-safety-function/3-safety-layout/3-safety-robot-modeling.md)
# 3.3.3.3 Safety Robot Modeling

A robot model used for safety space monitoring. Safety robot modeling can be applied to axes 2 and 3, and both are modeled as capsules.

The capsule used for the safety modeling for robots consists of the center and radius of the spheres at both ends. The center of the modeling sphere is the center position of the robot 2nd/3rd axis, and the radius should be large enough to include the size of the current link and the stop distance at the maximum TCP speed.

You can set parameter values   in the `[System > 10: Safety System > 2: Parameter setup > 2: Space restriction > 2: Robot]` menu.

<p align="center">
<img src="../../../_assets/safety_layout/robot.png"></img>
<em><p align="center">Safety Robot Modeling Settings Screen</p></em>
</p>

| **Parameter** |          **Description**                                     | **Default Setting** |
| :------: | --------------------------------------------------- | :--------: |
| <p>Height</p><p>[mm]</p> | <p>Plate height</p><p>(0 ~ 5000.0)</p> | 0 |
| <p>Radius</p><p>[mm]</p> | <p>Radius of sphere</p><p>(0 ~ 3000.0)</p> | 10 |
| <p>Center</p><p>[mm]</p> | <p>Center position</p><p>(-3000.0 ~ 3000.0)</p> | 0 |
| <p>Direction</p><p>[deg]</p> | <p>Orientation of coordinate system</p><p>(-180.0 ~ 180.0)</p> | 0 |                    |    0 mm    |

{% hint style="warning" %}
**\[Caution]**

* As the definition of robot layout settings applies only to the robot 2nd and 3rd axes, other parts of the robot may violate this area even if a safety area is set.
{% endhint %}
[__SOURCE](3-safety-function/3-safety-function/3-safety-layout/4-safety-tcp-orientation.md)
# 3.3.3.4 TCP Orientation Monitoring

To use the TCP orientation monitoring function, you can set up a monitoring cone by setting the rotation angle and deviation angle for generating the reference vector.

By setting the reference vector (![](../../../_assets/3.png)) by rotating the Z-direction vector of the robot coordinate system (![](../../../_assets/1.png)) by a set angle based on it, a cone (![](../../../_assets/2.png)) made up of mother lines that are separated by the deviation angle (![](../../../_assets/4.png)) can be modeled. The vertex of such a cone (![](../../../_assets/5.png)) is located at the TCP, and if the Z-direction vector of the TCP (![](../../../_assets/6.png)) crosses the monitoring cone, a TCP direction limit function violation error occurs.

<p align="center">
<img src="../../../_assets/safety_layout/tool_ori.png"></img>
<em><p align="center">TCP Orientation Monitoring</p></em>
</p>

You can set the parameter values   in the `[System > 10: Safety System > 2: Parameter setup > 2: Space restriction > 4: Tool orientation]` menu.

<p align="center">
<img src="../../../_assets/safety_layout/tool_orient_param.png"></img>
<em><p align="center">TCP Orientation parameter setting screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Whether the function is activated</p><p>(Invalid / Valid / Safe I/O)</p> | Invalid |
| Stop method | <p>Stop method in case of function violation</p><p>(Stop 0 / Stop 1 / Stop 2 / No stop)</p> | Stop 1 |
| <p>Org.Rx</p><p>[deg]</p> | <p>Rotation amount of reference vector relative to X direction</p><p>(-180.0 ~ 180.0)</p> | 0.0 |
| <p>Org.Ry</p><p>[deg]</p> | <p>Rotation amount of reference vector relative to Y direction</p><p>(-180.0 ~ 180.0)</p> | 0.0 |
| <p>Org.Rz</p><p>[deg]</p> | <p>Rotation of reference vector relative to Z direction</p><p>(-180.0 ~ 180.0)</p> | 0.0 |
| Deviation angle | <p>Tool orientation limit</p><p>(1.0 ~ 179.9)</p> | 0.0 |
| Load current position <br> | Create reference vector with current robot pose | - |


{% hint style="warning" %}
**\[Caution]**

* When changing tool data, be sure to recheck that the parameters set in safety tool modeling are accurate. The tool data number and safety tool modeling number of the same tool should match.
{% endhint %}

[__SOURCE](3-safety-function/3-safety-function/3-safety-layout/5-self-collision-detection.md)
# 3.3.3.5 Self-Collision Detection

Self-collision detection is a function that monitors potential collisions between Axis 2 of the robot and the tool.
The tool and the robot must be modeled to match their actual geometries.
For detailed information on the modeling methods, refer to "[3.3.3.2 Safety Tool Modeling](../../../3-safety-function/3-safety-function/3-safety-layout/2-safety-tool-modeling.md)" and "[3.3.3.3 Safety Robot Modeling](../../../3-safety-function/3-safety-function/3-safety-layout/3-safety-robot-modeling.md)".

<p align="center">
<img src="../../../_assets/safety_layout/self_collision.png"></img>
<em><p align="center">Self-Collision Detection</p></em>
</p>


You can set parameters for the robot's self-collision detection function in the `[System > 10: Safety System > 2: Parameter setup > 2: Space restriction > 5: Self-Collision Detection]` menu.

<p align="center">
<img src="../../../_assets/safety_layout/self_collision_param.png"></img>
<em><p align="center">Self-collision detection function parameter setting screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Whether the function is activated</p><p>(Invalid / Valid / Safe I/O)</p> | Invalid |
| Stop method | <p>Stop method when the function is violated</p><p>(Stop 0 / Stop 1 / Stop 2 / No stop)</p> | Stop 1 |





[__SOURCE](3-safety-function/3-safety-function/4-safety-io/README.md)
# 3.3.4 Safety Input/Output

Basic Information on Safety Input/Output

Hi7's safety input/output can be divided as follows:

- Basic Safety Input (4ch x dual input)
- Extended Safety Input (8ch x dual input)
- Basic Safety Output (1ch x dual input)
- Extended Safety Output (8ch x dual input)
- PROFIsafe Communication Safety Input (64 points)
- PROFIsafe Communication Safety Output (64 points)
- CIP Safety Communication Safety Input (64 points)
- CIP Safety Communication Safety Output (64 points)

![](../../../_assets/safety_io/comm_front.png)


[__SOURCE](3-safety-function/3-safety-function/4-safety-io/1-default-io.md)
# 3.3.4.1 Default Safety Input/Output Signals

Set the parameters for safety input/output signals.
There are 4 input signals and 1 output signal, all operating as dual signals.
You can set the parameter values in the `[System > 10: Safety System > 2: Parameter setup > 3: Safety I/O > 2: Default I/O]` menu. 

### 1) Default Input Signal Settings

<p align="center">
<img src="../../../_assets/safety_io/def_input.png"></img>
<em><p align="center">Default Input/Output Settings Screen (Input)</p></em>
</p>

| Parameter <br>[Unit]          | Description                                                                                                                                       | Input Range       | Default |
|:------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|:--------------:|:------:|
| Pulse Test                 | Set whether to use the Pulse Test for each channel. <br>For channels with the pulse test enabled, test pulses are sent to the input side as shown in the figure below. The cable condition is then verified by checking the received pulse signals.| Enable / Disable | Disable |
| Error Latch Time <br>[msec] | When an error occurs in a channel, even if the error is resolved, the system transitions from the Fail-Safe state to the current input state only after the **Error Latch Time** has elapsed.<br>Only values divisible by 10 can be entered. | 0 ~ 65530      | 1000   |
| Filter Time <br>[msec]      | The same signal should be input during the **Filter Time** set for each channel for it to be processed as a valid signal.<br>Only values divisible by 10 can be entered.                       | 0 ~ 500        | 100    |
| Discrete Time <br>[msec] | Basic input signals are processed as valid signals when two dual signals are identical.<br>An alarm is triggered if the two signals are different from each other for longer than the set **Discrete Time**.<br>Only values divisible by 10 can be entered. | 0 ~ 5000       | 1000   |

#### Input Test Pulse)
<p align="center">
<img src="../../../_assets/safety_io/Testpulse_Input.png"></img>
</p>

#### Wiring Example)
![](../../../_assets/safety_io/CN_SI1.bmp)


### 2) Output Signal Settings

<p align="center">
<img src="../../../_assets/safety_io/def_output.png"></img>
<em><p align="center">Default I/O Settings Screen (Output)</p></em>
</p>

| Parameter <br>[Unit]          | Description                                                                                                                                       | Input Range       | Default |
|:------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|:--------------:|:------:|
| Pulse Test                 | Configures whether the pulse test is used.<br> When the pulse test is enabled, the controller sends test pulses as shown in the figure below and determines the output status by verifying the received pulse signals. | Enable / Disable | Disable |
| Error Latch Time <br>[msec] | When an error occurs in a channel, even if the error is recovered, the system maintains the **Open (Fail-safe)** state during the **Error Latch Time**. Afterward, it  transitions to normal output.<br>Only values divisible by 5 can be entered. | 0 ~ 65530      | 1000   |


#### Output Test Pulse)
<p align="center">
<img src="../../../_assets/safety_io/Testpulse_output.png"></img>
</p>

#### Wiring Example)
![](../../../_assets/safety_io/CN_SO1.bmp)



[__SOURCE](3-safety-function/3-safety-function/4-safety-io/2-additional-io.md)
# 3.3.4.2 Extended Safety Input/Output Signals

Set the parameters for additional safety input/output signals. It consists of 8 input signals and 8 output signals, all operating as dual signals.
You can set parameter values in the `[System > 10: Safety System > 2: Parameter setup > 3: Safety I/O > 3: Additional I/O]` menu. 

### 1) Additional Safety Input/Output Signals

<p align="center">
<img src="../../../_assets/safety_io/add_io.png"></img>
<em><p align="center">Extended Input/Output Settings Screen</p></em>
</p>

| Parameter [Unit]             | Description                                                                                                                                       | Input Range       | Default |
|:---------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------:|:--------------:|:------:|
| Filter Time <br>[msec]          | For each input channel, constant signals should be input during the **Filter Time** for the signals to be processed as valid signals.<br>Only values divisible by 10 can be entered.                           | 0-500        | 100    |
| Discrepancy Time <br>[msec]     | Extended safety input/output signals are processed as valid signals when two dual signals have the same value.<br>An alarm is triggered if the two signals are different from each other for longer than the **Discrepancy Time**.<br>Only values divisible by 10 can be entered. | 0-5000       | 1000   |
| Input Error Latch Time <br>[msec] | When an error occurs in a channel, even if the error is resolved, the system transitions from the Fail-Safe state to the current input state only after the set time has elapsed.<br>Only values divisible by 10 can be entered.             | 0-65530      | 1000   |
| Output Error Latch Time <br>[msec] | When an error occurs in a channel, even if the error is resolved, the system maintains the **Open (Fail-safe)** state during the set time.<br>After that, it transitions to normal output.<br>Only values divisible by 10 can be entered.   | 0-65530      | 1000   |

#### Additional Safety Input Wiring Example)
![](../../../_assets/safety_io/CN_SI2.bmp)
#### Additional Safety Output Wiring Example)
![](../../../_assets/safety_io/CN_SO2.bmp)


[__SOURCE](3-safety-function/3-safety-function/4-safety-io/3-Linker.md)
# 3.3.4.3 Safety Signal Allocation

The Safety signal allocation function serves to connect external signals such as safety input/output, additional safety input/output, and safety communication input/output with various logical signals (system safety input/output, safety application signals) that the robot controller has.
You can set the parameter values in the `[System > 10: Safety System > 2: Parameter setup > 3: Safety I/O > 1: I/O Allocation]` menu.

![](../../../_assets/safety_io/SIO_Alloc_diagram1.bmp)

![](../../../_assets/safety_io/SIO_Alloc_diagram2.bmp)

-------------------------------------------------------------------------

### 1) Adding Safety Signal Allocation
1) Press the `[Add]` button.
2) Select the desired function from the function list.
3) If a sub-index is required, enter the sub-index number.

### 2) Deleting Safety Signal Allocation
1) Select an already set allocation function on the list.
2) Press the `[del]` button.

<p align="center">
<img src="../../../_assets/safety_io/io_alloc_param1.png"></img>
<em><p align="center">Safety Signal allocation Settings Screen</p></em>
</p>

{% hint style="warning" %}
* The Emergency Stop (EX_EM) and Safety Guard (SGG or SGA) signals are mandatory and must always be selected.<br>
* An individual input function item can only be connected to a single input channel.<br>
* "Basic Safety Input", "Additional Safety Input", and "Safety Communication Input" cannot be assigned in duplication mutually.<br>
* If duplicate input settings are made, the "E52030 (x ch) Safety input allocation duplication" error occurs.

{% endhint %}



### 3) Default values for safety signals

|  **Channel** |     **Function**                       | 
| :-------: | :------------------------------------------------: |
| Safety Input Channel 1 | External Emergency Stop Input (Emergency) |
| Safety Input Channel 2 | Safety Guard General Input (SGG)|
| Safety Input Channel 3 | - |
| Safety Input Channel 4 | - |
| Safety Output Channel 1 | Emergency Stop Activation Status|

### 4) Safety Input Signal Function List

|  **Channel** |     **Function**                       |       **Description**    |
| :-------: | :--------------------------: | :--------------------------------------------------: |
| Emergency | External Emergency Stop Input| OPEN: Emergency stop activated<br>CLOSE: Emergency stop released |
| SGG| Safety Guard General Input| OPEN: Guard open (Danger) <br>CLOSE: Guard closed (Safe) |
| SGA | Safety Guard Auto Input| OPEN: Guard open (Danger) <br>CLOSE: Guard closed (Safe) |
| Protective stop | Protective Stop Input | OPEN: Protective stop activated <br>CLOSE: Protective stop released |
| Normal stop | Normal Stop Input | OPEN: Normal stop activated <br>CLOSE: Normal stop released |
| Motor On | External Motor On | Motor On attempted on Rising Edge |
| Remote | External Mode Input (Remote) | OPEN: Mode change by internal mode signal <br>CLOSE: Mode change by external mode input signal
| Manual | External Mode Input (Manual)  | OPEN: No operation <br>CLOSE: External manual mode input |
| Auto | External Mode Input (Auto)  | OPEN: No operation <br>CLOSE: External auto mode input |
| Arm Limit | Arm Limit Input| OPEN: Limit signal input (Danger) <br>CLOSE: Limit signal closed (Safe) |
| Primary axis Limit | Primary Axis Limit Input | OPEN: Limit signal input (Danger) <br>CLOSE: Limit signal closed (Safe) |
| Additional axis Limit | Additional Axis Limit Input | OPEN: Limit signal input (Danger) <br>CLOSE: Limit signal closed (Safe) |
| External axis Limit | External Axis Limit Input | OPEN: Limit signal input (Danger) <br>CLOSE: Limit signal closed (Safe) |
| Monitored standstill #1-#8 | Monitored Standstill<br>(sos_0-sos_7) | OPEN: Function activated<br>CLOSE: Function deactivated |
| Joint speed set #1-#8 | Joint Speed<br>(speed_0-speed_7) | OPEN: Function activated<br>CLOSE: Function deactivated |
| TCP speed set #1-#16 | TCP Speed<br>(speed_0-speed_15) | OPEN: Function activated<br>CLOSE: Function deactivated |
| Joint angle #1-#8 | Joint Space<br>(space_0-space7) | OPEN: Function activated<br>CLOSE: Function deactivated |
| TCP position(space) #1-#16 | TCP Space<br>(space_0-space15) | OPEN: Function activated<br>CLOSE: Function deactivated |
| TCP orientation #1-#8 | Tool Orientation<br>(orient_0-orient7) | OPEN: Function activated<br>CLOSE: Function deactivated |
| Self collision | Self Collision | OPEN: Function activated<br>CLOSE: Function deactivated |
| Power #1-#16 | Power<br>(power_0-power_15) | OPEN: Function activated<br>CLOSE: Function deactivated |
| Momentum #1-#16 | Momentum<br>(mmt_0-mmt_15) | OPEN: Function activated<br>CLOSE: Function deactivated |
| Collision detection #1-#16 | Collision Detection<br>(coldet_0-coldet_15) | OPEN: Function activated<br>CLOSE: Function deactivated |
| RePlan #1-#4 | RePlan | OPEN: Function activated<br>CLOSE: Function deactivated |
| Mastering test switch | Mastering Test Switch | OPEN: Function activated<br>CLOSE: Function deactivated |

#### Safety Output Signal Function List
|  **Channel** |     **Function**                       |       **Description**    |
| :-------: | :--------------------------: |  :--------------------------------------------------: |
| Emergency stop activation status | Emergency Stop Status | OPEN: At least one of TP, OP, and external emergency stop is pressed <br> CLOSE: None of TP, OP, and external emergency stop is pressed.  |
| Protective stop activation status | Protective Stop Status | OPEN: Not in protective stop state<br> CLOSE: In protective stop state |
| Normal stop activation status | Normal Stop Status | OPEN: Not in normal stop state<br> CLOSE: In normal stop state |
| Remote mode status | External Operation Status | OPEN: Internal operation mode<br> CLOSE: External operation mode |
| Manual mode status | Manual Mode Status | OPEN: Not in manual mode <br> CLOSE: In manual mode |
| Auto mode status | Auto Mode Status | OPEN: Not in auto mode <br> CLOSE: In auto mode|
| Motor Off status | Motor Off Status | OPEN: Motor On state<br> CLOSE: Motor Off state|
| Safety Function activation status | Safety Function Activation Status | OPEN: Safety function deactivated<br> CLOSE: Safety function activated |
| Monitored standstill activation status | Safe Operating Stop Monitoring Activation Status | OPEN: Safe Operating Stop monitoring deactivated<br> CLOSE: Safe Operating Stop monitoring activated |
| Replan activation status | RePlan Activation Status | OPEN: RePlan deactivated<br> CLOSE: RePlan activated |
| Violation alarm | Safety Function Violation Status | OPEN: Safety function violated<br> CLOSE: No safety function violation |
| Monitored standstill #1-#8 violation | Safe Operating Stop Violation<br>(sos_0-sos_7) | OPEN: Safe Operating Stop violated<br> CLOSE: No Safe Operating Stop violation |
| Joint speed set #1-#8 violation | Joint Speed Violation<br>(speed_0-speed_7) | OPEN: Joint speed violated<br> CLOSE: No joint speed violation |
| TCP speed set #1-#16 violation | TCP Speed Violation<br>(speed_0-speed_15) | OPEN: TCP speed violated<br> CLOSE: No TCP speed violation |
| Joint angle #1-#8 violation | Joint Space Violation<br>(space_0-space7) | OPEN: Joint space violated<br> CLOSE: No joint space violation |
| TCP position #1-#16 violation | TCP Space Violation<br>(space_0-space15) | OPEN: TCP space violated<br> CLOSE: No TCP space violation |
| TCP orientation #1-#8 violation | Tool Orientation<br>(orient_0-orient7) | OPEN: Tool orientation violated<br> CLOSE: No tool orientation violation |
| Self collision detection | Self Collision Detection| OPEN: Self collision detected<br> CLOSE: No self collision |
| Power #1-#16 violation | Power Violation<br>(power_0-power_15) | OPEN: Power violated<br> CLOSE: No power violation |
| Momentum #1-#16 violation | Momentum Violation<br>(mmt_0-mmt_15) | OPEN: Momentum violated<br> CLOSE: No momentum violation |
| Collision detection #1-#16 violation | Collision Detection <br>(coldet_0-coldet_15) | OPEN: Collision detected<br> CLOSE: No collision |
| Mastering test error | Mastering Test Error | OPEN: Mastering test error occurred<br> CLOSE: No mastering test error |
| Brake test error | Brake Test Error | OPEN: Brake test error occurred<br> CLOSE: No brake test error |

{% hint style="info" %}
* Defined as **OPEN = Bit 0**, **CLOSE = Bit 1** in safety communication

{% endhint %}

[__SOURCE](3-safety-function/3-safety-function/4-safety-io/4-safe-comm-select.md)


# 3.3.4.4 Selecting Safety Communication

Select the safety communication protocol for the Hi7 robot controller.<br><br>
You can configure the parameter values in the `[System > 2: Control Parameters > 6: Safety Communication > 1: Select Safety Communication]` menu.

![](../../../_assets/safe_comm_select.png)

[__SOURCE](3-safety-function/3-safety-function/4-safety-io/5-profisafe.md)
<script id="page-config" type="application/json">
{
	"permittedStrs": ["HI6"]
}
</script>


# 3.3.4.5 PROFIsafe

### 1) PROFIsafe?
- A safety protocol (safety profile) that operates on PROFINET/PROFIBUS.
- Transmits safety data through standard PROFINET communication channels ('Black Channels').
- Supports safety signal transmission without the need for additional wiring.

### 2) PROFINET & PROFIsafe Specifications
- Digital Input: 50, 120, or 240 bytes (Select one)
- Digital Output: 50, 120, or 240 bytes (Select one)
- Safety I/O: 8/8 bytes (Enable or Disable)
- Minimum Communication Cycle: 1 msec
- Supported Communication Speed: 10 or 100 Mbps
- Conformance Class: B
- Netload Class: II
- Optional Features: Legacy, MRP

### 3) PROFIsafe Parameters

`[System > 2: Control Parameters > 11: Industrial Communication > 6: Safety Communication > 2: PROFIsafe]`<br>
![](../../../_assets/safetyio_profisafe/profisafe_param.png)

 - Source Address: Sets the Source Address. (Fixed to 1)
 - Target Address: Sets the Target Address. (Setting range: 1 to 65534)
 
 ***Note***<br> 
 - Address Type: Address Type 1 (Only Destination Address is allowed)
 - Reaction on Device_Fault: If this device enters a Fault state, all F-Outputs will change to the Fail-safe (0) state. Once the device's Fault state is resolved, a process of re-integrating the F-Device using a command such as Global-Acknowledge from the F-Host is required.
 

### 4) PROFIsafe Configuration Procedure

1) Connection between BD671 and F-Host & Hi7 Com
2) GSDML File Registration (TIA Portal)
3) PROFIsafe Controller Configuration (TIA Portal)
<br>3.1) PROFINET Configuration
<br>3.2) PROFIsafe Configuration
4) Hi7 Configuration (TP UI)
<br>4.1) PROFINET Configuration
<br>4.2) PROFIsafe Configuration
5) Verification of PROFINET and PROFIsafe Communication
6) Assignment of PROFINET I/O Signals (FB Block Settings)
7) Assignment of PROFIsafe I/O Signals


#### 4.1) Connection between BD671 and F-Host & Hi7 Com

##### 4.1.1) LAN Cable Connection
1) Connect the "PROFIsafe F-Host" and the BD671 using a LAN cable.
2) Verify that the Link LED is flashing.
3) Connect the LAN3 connector of the Hi7 COM and the BD671 using a LAN cable.
4) Verify that the Link LED is flashing.

![](../../../_assets/safetyio_profisafe/profisafe_connect.png)

##### 4.1.2) Hi7 Com Connection Settings
1) Navigate to the following menu: **System -> Control Parameters -> Industrial Communication -> EtherCAT Master Settings**
2) Configure the settings as follows:
- EtherCAT Master: ON
- Port: LAN3
3) Select "OptionBD - PROFINET_IO" from the slave list and press the **Apply** button.
4) Reboot the Hi7 robot controller.
5) After rebooting, check the status of the **Run**, **Communication**, and **Error** LEDs.

![](../../../_assets/safetyio_profisafe/EC_master_setting1.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/EC_master_setting2.png)


#### 4.2) GSDML File Registration (TIA Portal)
1) Launch TIA Portal.
2) Navigate to the menu as shown on the right: **[Options] → [Manage general station description file (GSD)]**.
3) Click the **"..."** button and select the directory where the GSDML file is located.
4) Select **"GSDML-V2.43-Hyundai-Robotics-HI6-20251127.xml"** from the list displayed on the screen and click the **[Install]** button.
5) Verify that the file has been registered as a new device in the Hardware Catalog. <br>
![](../../../_assets/safetyio_profisafe/profisafe_gsdmal.png)

#### 4.3) PROFIsafe Controller Configuration (TIA Portal)
##### 4.3.1) PROFINET Configuration
1) Launch TIA Portal and create a new project.
2) Double-click **Devices & Networks** to open it.<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network.png)

3) Select a controller that supports PROFIsafe communication (e.g., CPU 1511F-1 PN) and drag it into the **Network View**.
4) From the Hardware Catalog, select the device added in the previous step (HRC, PROFINET I/O DAP) and drag it into the **Network View**.
5) Connect the two devices by dragging and dropping between their respective LAN ports in the diagram.<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network2.png)

6) Double-click the HRC-IO device in the **"Devices & Networks"** view.
7) Select the desired slot.
8) Drag the desired module (DI, DO, or PROFIsafe I/O) from the catalog on the right and move it to the **"Device Overview"** window.<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network3.png)

9) Double-click the HRC-IO device in the **"Devices & Networks"** view.
10) Click the HRC-IO device again to open the **Properties** (Settings) window.
11) Navigate to the **General** tab at the bottom.
12) Select **Ethernet addresses** from the menu on the left.
13) Uncheck the **"Generate PROFINET device name automatically"** option.
14) Set the **"PROFINET device name"** to **"hd-hrc-hi7"** and save the changes.<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network4.png)

##### 4.3.2) PROFIsafe Configuration
1) Double-click the HRC-IO device in the **"Devices & Networks"** view.
2) Select the PROFIsafe slot in the **"Device Overview"** window on the right.
3) The PROFIsafe communication settings will appear in the bottom pane.
4) Click the **PROFIsafe** tab.
5) Set **F_Dest_Add** to 1.<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network5.png)

#### 4.4) Hi7 Configuration (TP UI)
##### 4.4.1) PROFINET Configuration
1) Configure the parameters with the same values set in the F-Host:
- PROFINET IO Device Name: hd-hrc-hi7
- Slot 1: Digital Input: 240
- Slot 2: Digital Output: 240
- Slot 3: Safety I/O: Selected
2) Press the **"Apply"** button.<br>
![](../../../_assets/safetyio_profisafe/4_1_profinet_config.png)

##### 4.4.2) PROFIsafe Configuration

1) Set the **Target Address** to 1, using the same value configured in the previous section.
2) Press the **"Apply"** button.<br>
![](../../../_assets/safetyio_profisafe/4_2_profisafe_config.png)

#### 4.5) Verification of PROFINET and PROFIsafe Communication

#### 4.5.1) Safety Ladder Program (TIA Portal)
1) In the **Device Overview** tab, create a ladder program as shown below and download it to the controller.<br>
![](../../../_assets/safetyio_profisafe/5_1_Safety_Ladder.png)
2) After downloading, verify that a green check box is displayed on the **Distributed I/O** screen.<br>
![](../../../_assets/safetyio_profisafe/5_1_Safety_Ladder2.png)

#### 4.5.2) TP Screen
1) PROFINET <br>
Navigate to **System -> 2: Control Parameters -> 11: Industrial Communication -> 5: PROFINET Settings** from the menu.<br>
![](../../../_assets/safetyio_profisafe/5_2_pnio_status.png)
- Check the status information for each slot.
- Verify that the Counter is continuously increasing.

2) PROFIsafe <br>
Navigate to **System > 2: Control Parameters > 11: Industrial Communication > 6: Safety Communication > 2: PROFIsafe** in the menu.<br>
![](../../../_assets/safetyio_profisafe/5_2_profisafe_status.png)
- Verify that **FappState** is set to **CYCLE Data EX**.
- Verify that the **Counter** is continuously increasing.

#### 4.6) Assignment of PROFINET I/O Signals (FB Block Settings)
1) Navigate to **System → Control Parameters → I/O Signal Settings → FB Block Assignment**.
2) Change the block settings to **PROFINET I/O** as needed, up to a maximum of 2 blocks.
 (The maximum PROFINET I/O size is 240 bytes, and each individual FB block size is 120 bytes. Therefore, **any settings exceeding 2 blocks will be ignored.**)<br>
![](../../../_assets/safetyio_profisafe/6_fb_block.png)

3) Additionally, navigate to the **Condition Settings** menu and verify that the **PLC Operation Mode** is set to **OFF**.<br>
![](../../../_assets/safetyio_profisafe/6_1_condition.png)
4) Verify the I/O signals in the **TIA Portal** and on the **General I/O** screen.<br>
![](../../../_assets/safetyio_profisafe/6_3_public_io.png)

#### 4.7) Assignment of PROFIsafe I/O Signals
1) Assignment of PROFIsafe I/O Signals
* Refer to the **[3.3.4.3 Safety Signal Assignment](../4-safety-io/3-Linker.md)** page.

2) Examples of PROFIsafe I/O Signal Assignment
<br>
<br>2-1) PROFIsafe Input (Direction: Master -> Slave)
<br><br>
[Set 0 bit as Arm Limit] <br>
![](../../../_assets/safetyio_profisafe/7_PS_in.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/7_PS_in2.png)
<br> <br>
2-2) PROFIsafe Output (Direction: Slave -> Master)
<br> <br>
[Set 0 bit as Emergency Stop State]<br>
![](../../../_assets/safetyio_profisafe/7_PS_out.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/7_PS_out2.png)




[__SOURCE](3-safety-function/3-safety-function/4-safety-io/6-cipSafety.md)


# 3.3.4.6 CIP Safety

### 1) What is CIP Safety?
- **CIP Safety** is a safety communication protocol that extends the standard **Common Industrial Protocol (CIP)**.
- It enables secure data exchange over **EtherNet/IP** and **DeviceNet** by utilizing the **"Black Channel"** principle.
- It complies with international safety standards such as **IEC 61508** and **ISO 13849** through mechanisms like time monitoring, redundancy, and CRC (Cyclic Redundancy Check).
<br>
<br>

### 2) Specifications
#### 2.1) EtherNet/IP
- **Digital Input:** 0 ~ 240 bytes
- **Digital Output:** 0 ~ 240 bytes
- **RPI (Requested Packet Interval):** 5 ~ 3000 msec
- **Supported Communication Speed:** 10 or 100 Mbps

#### 2.2) CIP Safety
- **Safety I/O:** 8/8 bytes
- **RPI (Requested Packet Interval):** 20 ~ 100 msec
<br>
<br>

### 3) CIP Safety Parameters
`[System > 2: Control Parameters > 11: Industrial Communication > 6: Safety Communication > 3: CIP Safety]`<br>
![](../../../_assets/cipSafety/cipSafety_Parameters.png)

 - **Safety Network Number:** Sets the Safety Network Number (SNN).
 - **IP Address:** Displays the currently configured IP address of the EtherNet/IP Adapter.
 <br>{% hint style="info" %}
* If the IP address of the EtherNet/IP Adapter is changed, you must execute **"Apply All"** for the CIP Safety parameters.
{% endhint %}
 
   

### 4) CIP Safety Configuration Procedure

1) Establish connection between Hi7 EtherNet/IP Adapter and EtherNet/IP Scanner.
2) Add EDS file via engineering tool (Studio 5000).
3) Configure CIP Safety Controller (Studio 5000).
4) Configure Hi7 (TP UI).
   4.1) EtherNet/IP Configuration
   4.2) CIP Safety Configuration
5) Verify EtherNet/IP and CIP Safety communication status.
6) Assign safety signals.


#### 4.1) Connection between Hi7 EtherNet/IP Adapter and EtherNet/IP Scanner
![](../../../_assets/cipSafety/connect.png)

#### 4.2) Adding EDS File via Engineering Tool (Studio 5000)
- Install the EDS file (**Hi7_EIP_251023.eds**) using the **'Device Description File Installation Tool'**.

#### 4.3) CIP Safety Controller Configuration (Studio 5000)
1) Launch **Studio 5000** and create a new project.
2) In the **Controller Organizer**, select a controller that supports CIP Safety communication (e.g., CPU 1769-L30ERMS). Right-click on **Ethernet** and click **New Module**.
3) Search for **"Hi7 EIP Adapter"** and click the **Create** button.<br>
![CIP Safety](../../../_assets/cipSafety/new_module.png)

4) Enter the device name in the **Name** field.
5) Set the **IP Address** (e.g., 192.168.4.150).
6) Set the **Safety Network Number** (e.g., 1111_2222_3333).<br>
![CIP Safety](../../../_assets/cipSafety/Setting_SNN.png)


7) Click the **Change** button in the **Module Definition** to configure the sizes for Safety I/O and Standard I/O.
- **Standard I/O (Exclusive Owner):** 240 bytes
- **Safety I/O:** 8 bytes each
8) Do not configure the **"Configuration signature"**.
9) Close the **Select Module Type** window.<br>
![CIP Safety](../../../_assets/cipSafety/Setting_module.png)

10) Verify that the module has been added successfully.<br>
![CIP Safety](../../../_assets/cipSafety/module_added.png)

11) Click the **Offline** button in the toolbar menu and then click **Download**.<br>
![CIP Safety](../../../_assets/cipSafety/download.png)

12) After the configured values are downloaded, switch the **GuardLogix** toggle from **PROG** to **RUN** mode.

#### 4.4) Hi7 Configuration (TP UI)
##### 4.4.1) EtherNet/IP Configuration
1) Navigate to **System → Control Parameters → Industrial Communication → EtherNet/IP Settings**.
2) Set **Protocol** to **Adapter**.
3) Set the LAN port for the EtherNet/IP Adapter to **LAN2**.
4) Set both **Input** and **Output** sizes to **240 bytes** each.
5) Do not change the remaining settings, leaving them as shown in the figure.<br>
![CIP Safety](../../../_assets/cipSafety/ethernetIP.png)

##### 4.4.2) CIP Safety Configuration
1) Navigate to **System → 2: Control Parameters → 11: Industrial Communication → 6: Safety Communication → 3: CIP Safety**.
2) Set the **Activation** button to **ON**.
3) Set the **SNN** (e.g., 1111_2222_3333) to match the value configured in Studio 5000.
4) Click the **Apply** button.
5) **Reboot** the robot controller.<br>
![CIP Safety](../../../_assets/cipSafety/cipSafety_Parameters.png)

#### 4.5) Verifying Communication Status
##### 4.5.1) EtherNet/IP
1) Verify that the **License LED** is lit.
2) Verify that the **Run LED** is lit.
3) Verify that the **Communication LED** is lit.
4) If the **Error LED** is lit, check the **Error Name** for details.<br>
![CIP Safety](../../../_assets/cipSafety/eip_status.png)

##### 4.5.2) CIP Safety
1) Verify that **Safety Communication** is set to **"CIP Safety"**.
2) Verify that the **Comm status** is in **"On-line, Connected"** state.
3) Verify that the **IO Count** is continuously increasing.<br>
![CIP Safety](../../../_assets/cipSafety/cipsafety_status.png)

#### 4.6) Safety Signal Assignment
##### 4.6.1) Assignment of CIP Safety I/O<br>
* Refer to the **[3.3.4.3 Safety Signal Assignment](../4-safety-io/3-Linker.md)** page.

##### 4.6.2) Examples of CIP Safety I/O Assignment
1) CIP Safety Input (Direction: Master -> Slave)
1ch(0 bit) = Arm Limit<br>
![CIP Safety](../../../_assets/cipSafety/alloc_in.png)<br>
<br> <br>
![CIP Safety](../../../_assets/cipSafety/alloc_in2.png)<br>

2) CIP Safety Output (Direction: Slave -> Master)
1ch(0 bit) = E-Stop Status<br>
![CIP Safety](../../../_assets/cipSafety/alloc_out.png)<br>
<br> <br>
![CIP Safety](../../../_assets/cipSafety/alloc_out2.png)<br>


[__SOURCE](4-configuration/README.md)
# 4. Function Settings


[__SOURCE](4-configuration/1-check-before-configuration/README.md)
# 4.1 Items to Check Before Using Safety Functions


[__SOURCE](4-configuration/1-check-before-configuration/3-password-setting.md)
# 4.1.1 Password Setting

The safety function parameters must be set and managed by a designated person. Users designated as administrators are granted administrator privileges and a system setting password. The system setting password is a required input item when setting the safety function parameters, and the parameters cannot be changed or set if the password is incorrect.

1. Tap the `[System > 5: Initialization > 11: System password setting]` menu. The password setting window will appear.
2. Enter the password and touch the `[OK]` button.

<p align="center">
<img src="../../_assets/4/password_setting.png"></img>
<em><p align="center">Password setting screen</p></em>
</p>

* When setting then safety function parameters, you must enter the system setting password to save changes.

{% hint style="warning" %}
* It is recommended to set the password with 4 or more characters.
* If you lose your password, contact an engineer.
* The default password is '8426'. 
{% endhint %}

[__SOURCE](4-configuration/1-check-before-configuration/1-encoder-offset.md)
# 4.1.2 Encoder Inspection

Since the safety function diagnoses the robot's position and speed based on the data of the encoder mounted on each axis, the accuracy of the encoder data is important. Therefore, you should check whether the encoder values match the actual values before using the safety function.

1\. Check the home position mark of each robot axis and move the axis.


When a stop occurs due to a safety function violation, move each axis by jogging in manual mode. For detailed information on recovery methods, refer to "[6.1 Recovery Mode](../../6-recovery/README.md)".

2\. In the pose information window in the work area, verify that the robot's axis coordinate values are displayed as the reference posture (**0, 90, 0, 0, 0, 0** \[deg]).


* If there is no pose information window in the work area, touch the `[+]` button at the upper right of the panel stack, then touch `[Pose]` in the panel selection window.


3\. If the angle value error is within 0.01, proceed to the next step. If the error exceeds 0.01, perform encoder offset.

4\. Reboot the system.

{% hint style="info" %}
For more information about encoder offset, see "[7.4.4 Encoder Offset](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/ko-tp630/README?cont_model=Hi7)" in the "[Hi7 Controller Operating Manual](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/ko-tp630/7-system/4-robot-parameter/4-encoder-offset/README?cont_model=Hi7)".
{% endhint %}

[__SOURCE](4-configuration/1-check-before-configuration/2-tool-data-setting.md)
# 4.1.3 Tool Data Setting

Safety features monitor the entire robot system, including tools attached to the robot flange. Therefore, the smaller the error between the tool data and actual values, the more accurately the safety function operates. Set the tool length and angle based on the flange coordinate system and enter the tool weight, center of gravity, and inertia information in accordance with individual units.

1. Set the operation mode to manual mode.
2. Press the emergency stop switch to cut off the power to the motors.
3. Touch the `[Settings]` button > `[3: Robot Parameters > 1: Tool Data]` menu.
4. Check the data for each axis and set the tool weight, center of gravity, and inertia, then touch the `[OK]` button to save.
5. Apply the updated tool data to the safety tool data. For more information about safety tool data, see "[3.3.1.3 Safety Tool Information](../../3-safety-function/3-safety-function/1-general-condition/3-safe-tool-info.md)".

{% hint style="info" %}
* If information about the tool's weight and center of gravity isn't available, you can use the load estimation function to estimate the values. 
* For detailed information on setting tool data, refer to the "[7.4.1 Tool Data](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/en-tp630/7-system/4-robot-parameter/1-tool-data/README?cont_model=Hi7)" in the "[Hi7 Controller Operation Manual](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/en-tp630/README?cont_model=Hi7)."
{% endhint %}

[__SOURCE](4-configuration/2-test-safety-functions.md)
# 4.2 Safety Function Test

When the robot system is installed and configured for the first time, or whenever robot components are replaced or optional devices are added or modified, the relevant safety functions shall be tested and validated in accordance with the procedures described below before the robot system is put into operation.


### 1. Emergency Stop

| Step | Test Procedure                                                                               | Expected Result                                      |
| ---- | -------------------------------------------------------------------------------------------- | ---------------------------------------------------- |
| 1    | Check that there is no visible damage or abnormality on the robot and the robot controller.  | No abnormalities are found.                          |
| 2    | Verify that the Emergency Stop button is released.<br>(Turn it clockwise until it pops out.) | Emergency Stop released.                             |
| 3    | Turn on the power to the robot controller.                                                   | The controller starts up.                            |
| 4    | In Manual mode, operate the Enabling Switch to change to the **Motor ON** state.             | The **Motor ON** indicator on the TP is illuminated. |
| 5    | Press the Emergency Stop button.                                                             | An Emergency Stop input is detected.                 |
| 6    | Verify that the system has changed to the **Motor OFF** state.                               | **Motor OFF** state.                                 |


**Acceptance Criteria**

* Pressing the Emergency Stop button shall cause the system to transition to the **Motor OFF** state.
* The **Motor ON** indicator on the TP shall blink or turn off.
* The robot shall not be operable while the Emergency Stop condition is active.


<br>

### 2. Safeguard General Signal (SGG)

| Step | Test Procedure                                                                              | Expected Result                                                |
| ---- | ------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| 1    | Check that there is no visible damage or abnormality on the robot and the robot controller. | No abnormalities are found.                                    |
| 2    | Verify that the safeguard signal is inactive. (Example: The safety fence door is closed.)   | Safeguard signal is in the normal state. (System Input screen) |
| 3    | Turn on the power to the robot controller.                                                  | The controller starts up.                                      |
| 4    | In Manual mode, operate the Enabling Switch to change to the **Motor ON** state.            | The **Motor ON** indicator on the TP is illuminated.           |
| 5    | Activate the safeguard signal. (Example: Open the safety fence door.)                       | Safeguard signal input is detected.                            |
| 6    | Verify that the system has changed to the **Motor OFF** state.                              | **Motor OFF** state.                                           |

**Acceptance Criteria**

* Activating the safeguard signal shall cause the system to transition to the **Motor OFF** state.
* The **Motor ON** indicator on the TP shall blink or turn off.
* The robot shall not be operable while the safeguard signal is active.


<br>

### 3. Safeguard Automatic Signal (SGA)

| Step | Test Procedure                                                                              | Expected Result                                                |
| ---- | ------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| 1    | Check that there is no visible damage or abnormality on the robot and the robot controller. | No abnormalities are found.                                    |
| 2    | Verify that the safeguard signal is inactive. (Example: The safety fence door is closed.)   | Safeguard signal is in the normal state. (System Input screen) |
| 3    | Turn on the power to the robot controller.                                                  | The controller starts up.                                      |
| 4    | In **Automatic** mode, change to the **Motor ON** state.                                    | The **Motor ON** indicator on the TP is illuminated.           |
| 5    | Open the safeguard. (Example: Open the safety fence door.)                                  | Safeguard signal input is detected.                            |
| 6    | Verify that the system has changed to the **Motor OFF** state.                              | The **Motor ON** indicator on the TP blinks or turns off.      |

**Acceptance Criteria**

* Activating the safeguard signal in **Automatic** mode shall cause the system to transition to the **Motor OFF** state.
* The **Motor ON** indicator on the TP shall blink or turn off.
* The robot shall not be operable while the safeguard signal is active.


<br>

### 4. Enabling Switch

| Step | Test Procedure                                                                                 | Expected Result                                           |
| ---- | ---------------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| 1    | Check that there is no visible damage or abnormality on the robot and the robot controller.    | No abnormalities are found.                               |
| 2    | Turn on the power to the robot controller.                                                     | The controller starts up.                                 |
| 3    | In **Manual** mode, hold the **Enabling Switch** in the middle position (**Enable Position**). | Enabling state is active.                                 |
| 4    | Verify that the system is in the **Motor ON** state.                                           | The **Motor ON** indicator on the TP is illuminated.      |
| 5    | Release the **Enabling Switch**. <br> or  Squeeze the **Enabling Switch** fully.                   | Enabling is deactivated.                                  |
| 6    | Verify that the system has changed to the **Motor OFF** state.                                 | The **Motor ON** indicator on the TP blinks or turns off. |

**Acceptance Criteria**

* Releasing the **Enabling Switch** shall cause the system to transition to the **Motor OFF** state.
* The **Motor ON** indicator on the TP shall blink or turn off.
* The robot shall not be operable while the **Enabling Switch** is released.


<br>

### 5. 비상정지 출력

| 단계 | 시험 절차                               | 예상 결과       |
| -- | ----------------------------------- | ----------- |
| 1  | 로봇 및 로봇제어기에 외관상의 손상이나 이상이 없는지 확인한다. | 이상 없음       |
| 2  | 모든 비상정지 버튼(TP, OP)이 복귀된 상태인지 확인한다.  | 비상정지 해제 상태  |
| 3  | 로봇제어기의 전원을 투입한다.                    | 제어기 기동      |
| 4  | 비상정지 출력이 활성화 상태인지 확인한다.             | 비상정지 출력 활성(출력 LED 점등 확인)  |
| 5  | TP의 비상정지 버튼을 누른다.                   | 비상정지 입력 발생  |
| 6  | 비상정지 출력이 비활성화 상태로 전환되는지 확인한다.       | 비상정지 출력 비활성(출력 LED 소등 확인) |

**합격 기준**

* 모든 비상정지 버튼이 복귀된 상태에서는 비상정지 출력이 활성화되어야 한다.
* TP 또는 OP의 비상정지 버튼을 누르면 비상정지 출력이 비활성화되어야 한다.
* 비상정지 상태가 유지되는 동안 비상정지 출력은 비활성 상태를 유지하여야 한다.

<br>

### 6. 기본 및 부가 안전 입력

**사전 조건 (Pre-condition)**

* 안전기능 할당 설정에서 시험 대상 입력 채널에 비상정지(E-Stop) 기능이 할당되어 있어야 한다.

| 단계 | 시험 절차                                         | 예상 결과                              |
| -- | --------------------------------------------- | ---------------------------------- |
| 1  | 로봇 및 로봇제어기에 외관상의 손상이나 이상이 없는지 확인한다.           | 이상 없음                              |
| 2  | 비상정지 버튼이 복귀된 상태인지 확인한다.                       | 비상정지 해제 상태                         |
| 3  | 로봇제어기의 전원을 투입한다.                              | 제어기 기동                             |
| 4  | 수동 모드에서 Enabling Switch를 조작하여 모터 ON 상태로 전환한다. | TP의 Motor ON 표시등 점등                |
| 5  | 시험 대상 안전 입력에 연결된 비상정지 버튼을 누른다.                | 비상정지 입력 발생                         |
| 6  | 모터 OFF 여부를 확인한다.                              | TP의 Motor ON 표시등이 점멸 또는 소등 상태로 변경됨 |

**합격 기준**

* 시험 대상 안전 입력에 비상정지 신호가 입력되면 모터 전원이 차단되어야 한다.
* TP의 Motor ON 표시등이 점멸 또는 소등 상태로 변경되어야 한다.
* 비상정지 상태에서는 로봇이 구동되지 않아야 한다.

<br>

### 7. 기본 및 부가 안전 출력

**사전 조건 (Pre-condition)**

* 안전기능 할당 설정에서 시험 대상 출력 채널에 비상정지 출력(E-Stop Output) 기능이 할당되어 있어야 한다.

| 단계 | 시험 절차                               | 예상 결과          |
| -- | ----------------------------------- | -------------- |
| 1  | 로봇 및 로봇제어기에 외관상의 손상이나 이상이 없는지 확인한다. | 이상 없음          |
| 2  | 모든 비상정지 버튼(TP, OP)이 복귀된 상태인지 확인한다.<br>(시계방향 회전 시켜 돌출 확인)   | 비상정지 해제 상태     |
| 3  | 로봇제어기의 전원을 투입한다.                    | 제어기 기동         |
| 4  | 시험 대상 안전 출력이 활성화 상태인지 확인한다.         | 비상정지 출력 활성 상태(출력 LED 점등 확인)  |
| 5  | TP의 비상정지 버튼을 누른다.                   | 비상정지 입력 발생     |
| 6  | 시험 대상 안전 출력이 비활성화 상태로 전환되는지 확인한다.   | 비상정지 출력 비활성 상태(출력 LED 소등 확인) |

**합격 기준**

* 모든 비상정지 버튼이 복귀된 상태에서는 시험 대상 안전 출력이 활성화 상태여야 한다.
* TP 또는 OP의 비상정지 버튼이 눌리면 시험 대상 안전 출력이 비활성화 상태로 전환되어야 한다.
* 비상정지 상태가 유지되는 동안 시험 대상 안전 출력은 비활성 상태를 유지하여야 한다.

<br>

### 8. 브레이크 테스트

| 단계 | 시험 절차                               | 예상 결과              |
| -- | ----------------------------------- | ------------------ |
| 1  | 로봇 및 로봇제어기에 외관상의 손상이나 이상이 없는지 확인한다. | 이상 없음              |
| 2  | 로봇제어기의 전원을 투입한다.                    | 제어기 기동             |
| 3  | 브레이크 테스트 Job 프로그램을 불러온다.            | 프로그램 정상 로드         |
| 4  | 조작 모드를 자동 모드로 변경한다.                 | 자동 모드 변경 확인        |
| 5  | 모터 ON 버튼을 입력한다.                     | 모터 ON 상태로 전환됨      |
| 6  | 시작 버튼을 입력한다.                        | 브레이크 테스트 프로그램이 실행됨 |
| 7  | 프로그램 종료 여부를 확인한다.                   | 브레이크 테스트 정상 종료     |

**합격 기준**

* 브레이크 테스트 프로그램 실행 중 모터 ON 상태가 유지되어야 한다.
* 브레이크 테스트 프로그램 실행 중 에러가 발생하지 않아야 한다.
* 브레이크 테스트 프로그램이 정상적으로 종료되어야 한다.
<br>"[로봇언어 HRScript](https://hrbook-hrc.web.app/#/view/doc-hrscript/ko/10-etc/1-proc/16-brake_check?cont_model=Hi7)" 참고





[__SOURCE](4-configuration/3-change-safety-parameter.md)
# 4.2 Safety Parameter Transfer

You can edit safety parameter values   and apply them to the system. Any values   that haven't been transferred will be reset when you exit the settings screen.

1. Go to `[System > 10: Safety System]` and select the menu you want to change.

<p align="center">
<img src="../_assets/4/apply_parameter_1.png"></img>
<em><p align="center">Example of entering the safety parameter setting screen</p></em>
</p>

2. If you have multiple pages, navigate to the page you wish to edit. The values   entered on each page are temporarily saved. (If you exit the menu without clicking "Apply to All," the changes will not be reflected.)

3. Enter the desired values   and click the `[Apply to All]` button.

<p align="center">
<img src="../_assets/4/apply_parameter_2.png"></img>
<em><p align="center">Safety parameter setting example</p></em>
</p>

4. Enter the password set in the system.

<p align="center">
<img src="../_assets/4/apply_parameter_3.png"></img>
<em><p align="center">Password input screen</p></em>
</p>

5. If you enter the correct password, the parameters will be transmitted. Check the transmission results.

<p align="center">
<img src="../_assets/4/apply_parameter_4.png"></img>
<em><p align="center">Output screen when transmission is successful</p></em>
</p>

{% hint style="warning" %}
**\[Warning]** : Before using the robot application, all safety parameters shall be verified and confirmed.

* Verification of safety parameters is an essential procedure to ensure that the safety functions operate as intended.
* Verification and validation shall be performed not only during initial setup but also after any modification of the parameters.
* Failure to verify safety parameters may result in safety functions not operating as intended and may pose a risk to personnel.
{% endhint %}
[__SOURCE](4-configuration/4-safety-parameter-report.md)
# 4.3 Safety Parameter Report

You can view the currently applied safety parameter values in a report format.
If the values on the settings screen have not been saved, they may differ from the values shown in the report.

1. Go to the menu you want to modify under `[System > 10: Safety System]`.

<p align="center">
<img src="../_assets/4/safety_report__1.png"></img>
<em><p align="center">Example of entering the safety parameter setting screen</p></em>
</p>

2. To generate a report, click the **\[Report]** button at the bottom.

<p align="center">
<img src="../_assets/4/safety_report__2.png"></img>
<em><p align="center">Example of generating a report</p></em>
</p>

3. The report will be created and displayed on the screen.

<p align="center">
<img src="../_assets/4/safety__report_3.png"></img>
<em><p align="center">Example of the report display screen</p></em>
</p>

4. If you want to save the generated report, click the **\[Print]** button.

<p align="center">
<img src="../_assets/4/safety__report_4.png"></img>
<em><p align="center">Example of the report print screen</p></em>
</p>

5. The password entry screen will appear. Enter the correct password.

<p align="center">
<img src="../_assets/4/safety_report_5.png"></img>
<em><p align="center">Example of the password entry screen</p></em>
</p>

6. If the correct password is entered, the report will be saved and a notification window indicating that the save is complete will be displayed.

<p align="center">
<img src="../_assets/4/safety_report_6.png"></img>
<em><p align="center">Example of the report save completion screen</p></em>
</p>

{% hint style="info" %}
* Safety parameters are protected by an identifier (CRC) to ensure integrity.
* The identifier is calculated based on all safety parameters and includes parameters related to all safety functions.
* When safety parameters are modified, the identifier value is also changed, and the identifier value can be checked in the CRC field of the safety parameter report.
* The identifier uniquely identifies the set of included safety functions and their associated parameters.
{% endhint %}
[__SOURCE](5-monitoring/README.md)
# 5. Safety Status Monitoring

Monitors safety function violations, safety I/O and safety communication status. 

You can check the information of the status of robot monitoring functions and safety I/O in the `[System > 10: Safety System > 3: Monitoring]` menu.

The status of safety communication can be checked in the `[System > 2: Control Parameters > 11: Industrial Communication > 6: Safety Communication]` menu.

[__SOURCE](5-monitoring/1-robot-limit-parameter-monitoring.md)
# 5.1 Robot Monitoring Function Monitoring

You can check the robot TCP speed/TCP position/TCP direction/power/momentum status by selecting the `[System > 10: Safety System > 3: Monitoring > 1: Robot Status]` menu.


<p align="center">
<img src="../_assets/5/robot_mon.png"></img>
<em><p align="center">Robot status monitoring screen</p></em>
</p>

* Check the status of the robot monitoring function.
  * **\[TCP Position]**: TCP position monitoring violation status
  * **\[TCP Speed]**: TCP speed monitoring violation status
  * **\[TCP Orientation]**: TCP orientation monitoring violation status
  * **\[Power]**: Power monitoring violation status
  * **\[Momentum]**: Momentum monitoring violation status

---

You can check joint area/speed/SOS/collision status by selecting the `[System > 10: Safety System > 3: Monitoring > 2: Joint Status]` menu.

<p align="center">
<img src="../_assets/5/joint_mon.png"></img>
<em><p align="center">Joint Status Monitoring Screen</p></em>
</p>

* Check the status of the joint limit function.
* **\[Joint Area]**: Whether joint area monitoring is violated.
* **\[Joint Speed]**: Whether joint speed monitoring is violated.
* **\[Collision]**: Whether collision monitoring is violated.
* **\[SOS]**: Whether (Safety Stop Monitoring) SOS monitoring is violated.

[__SOURCE](5-monitoring/4-safety-io-status-monitoring.md)
# 5.2 Safety I/O Status

You can monitor the system's basic/extended safety I/O status by selecting the `[System > 10: Safety System > 3: Monitoring > 3: Safety I/O Status]` menu.

<p align="center">
<img src="../_assets/5/safetyIO_mon.png"></img>
<em><p align="center">Safety input/output status monitoring screen</p></em>
</p>




[__SOURCE](5-monitoring/6-profisafe-status-monitoring.md)
# 5.3 PROFIsafe Monitoring

You can monitor the I/O status of PROFIsafe by selecting the `[System > 2: Control Parameters > 11: Industrial Communication > 6: Safety Communication > 2: PROFIsafe]` menu.

<p align="center">
<img src="../_assets/safetyio_profisafe/5_2_profisafe_status.png"></img>
<em><p align="center">PROFIsafe Status Monitoring Screen</p></em>
</p>

- **FappState:**<br>
CYCLIC_DATA_EX : PROFIsafe communication is running. <br>
NO_CYCLIC_DATA_EX : The PROFIsafe application is running, but PROFIsafe communication has not started. <br>
- **F-Parameter**
- **Config**
- **I/O Count:** (Number of I/O transmissions/receptions)

[__SOURCE](5-monitoring/7-cipsafety-status-monitoring.md)
# 5.4 CIP Safety Monitoring

You can monitor the I/O status of CIP Safety by navigating to the `[System > 2: Control Parameters > 11: Industrial Communication > 6: Safety Communication > 3: CIP Safety]` menu.

<p align="center">
<img src="../_assets/cipSafety/cipsafety_status.png"></img>
<em><p align="center">CIP Safety Monitoring</p></em>
</p>

- **Device Status:** <br>
Executing : CIP Safety communication is running. <br>
Idle : CIP Safety application is running, but CIP Safety communication has not started. <br>
Abort : Initial step Error<br>
Fault : Critical Error<br>
Configuring : Applying Configuration data failed<br>
- **Communication Status:**<br>
Connection Fail : A connection failure has occurred.
On-Line, Connected : Link is OK. The device is online and connected to Originator.
On-Line, No Conn : The device is online but not connected to Originator.
- **I/O Count:** (Number of I/O transmissions/receptions)

[__SOURCE](6-recovery/README.md)
# 6. Recovery

Errors caused due to safety function monitoring violations are cleared when switching to manual mode. In manual mode, safety function violations do not stop the robot, so, you can adjust the robot's angle and position to move it to a safe area.


{% hint style="warning" %}
**\[Caution]**: After recovery in manual mode, recheck the safety function settings and teaching positions of the work program.
{% endhint %}

[__SOURCE](6-recovery/1-recovery-robot-position-violation.md)
# 6.1 	Recovery from Robot Position Violation

Robot position violation occurs when the robot's position leaves the safety area, and the violations include TCP position violation, TCP orientation violation, and joint monitoring violation. In case of robot position violation, the error can only be cleared by physically moving the robot to change its position.

1. Change the mode switch to manual to enter manual mode.


2. Use the enabling switch on the teach pendant to turn on the motor.


3. Use the teach pendant to move the robot to a safe area.


4.  In the safety status monitoring screen, verify that the status of each area is displayed as **SAFE**.


{% hint style="warning" %}
After clearing the error, recheck the safety layout settings and also the teaching positions in the work program.
{% endhint %}

[__SOURCE](6-recovery/2-recovery-robot-speed-violation.md)
# 6.2 	Recovery from Robot Speed Violation

Robot speed violation including the TCP speed, joint speed, power, and momentum monitoring violations occurs when the robot's speed exceeds the safety standards,. In case of robot speed violation, the robot detects momentary speed and stops, so the error can be cleared without moving the robot's position.

1. Change the mode switch to manual to enter manual mode.


2.  In the safety status monitoring screen, verify that the status of each area is displayed as **SAFE**.


{% hint style="warning" %}
**[Caution]**

* After clearing the error, be sure to check the speed-related safety parameters and the speed of the work program.
{% endhint %}

[__SOURCE](6-recovery/3-recovery-robot-force-violation.md)
# 6.3 	Recovery from Robot Force Violation

Robot force violation such as collision detection, power, and momentum monitoring violations occurs when external force is applied or the magnitude of force used inside the robot exceeds the safety standards,. Depending on the cause of the violation, the error can be cleared.

<mark style="color:green;">**When violation occurs due to external force applied to the robot**</mark>

1. Remove external factors applying force to the robot.


2. Change the mode switch to manual to enter manual mode.


3.  In the safety status monitoring screen, verify that the status of each area is displayed as **SAFE**.


{% hint style="warning" %}
**\[Caution]**

* After clearing the error, recheck the safety function settings, tool data, and work program's teaching positions and speed.
{% endhint %}

[__SOURCE](6-recovery/4-recovery-sos-violation.md)
# 6.4 	Recovery from Safe Operating Stop (SOS) Violation

Safe Operating Stop (SOS) violation occurs when movement is detected while the robot motor is on and in a stopped state. In case of safe operating stop violation, the robot detects momentary movement and generates an error, so the error can be cleared without moving the robot's position.

1. Change the mode switch to manual to enter manual mode.


2. Remove external factors that apply force to the robot.


3. In the safety status monitoring screen, verify that the status of each area is displayed as **SAFE**.


{% hint style="warning" %}
**[Caution]**

* After clearing the error, check the safe operating stop monitoring parameters.
* Turn on the motor in auto mode and check whether the error recurs.
* If the same error occurs again, inspect the motor and reducer of the corresponding axis.
{% endhint %}

[__SOURCE](7-error-message/README.md)
# 7. Error Messages

When a safety function-related alarm occurs, refer to "[Error and Warning Help](https://hr-alarms.web.app/#/)".

[__SOURCE](attachment/README.md)
# Appendix


[__SOURCE](attachment/add-new-robot-model.md)
# Registering a New Robot Model

****

1. From the robot modeling files located in the library within the HRSpace installation directory, copy the folder of the robot model you want to use.
* File path: [HRSpace(version)\Library\Robot]

2. Add the copied folder to the robot 3D file storage directory of the controller.
* File path: [prebuilt\tp\libs3d\robot]

3. If the name of the folder containing the robot 3D files corresponds to an older version, rename it to the new version.

****

* Example: Adding a New HS220S Robot Model

1) Copy the HS220S robot modeling file from the robot modeling files stored in the library.

<p align="center">
<img src="../_assets/add_new_robot_model/add_new_robot_model_1.png"></img>
<em><p align="center">Check the location of the robot modeling file to be added and copy it</p></em>
</p>

2) Save the copied folder to the robot 3D file storage directory of the controller.

<p align="center">
<img src="../_assets/add_new_robot_model/add_new_robot_model_2.png"></img>
<em><p align="center">Paste the copied folder into the controller's robot 3D file storage directory</p></em>
</p>

3) Change the folder name to the new version.

<p align="center">
<img src="../_assets/add_new_robot_model/add_new_robot_model_3.png"></img>
<em><p align="center">If the robot modeling folder name corresponds to an older version, rename the folder</p></em>
</p>

[__SOURCE](attachment/rules-criteria-and-public-notice.md)
# Industrial Safety and Health Standards Rules and Safety Inspection Notice

The industrial robot in question should be installed in consideration of the inspection standards of the Industrial Safety and Health Standards Rules and Safety Inspection Notice (if subject to inspection).

"[Rules on Industrial Safety and Health Standards](https://hrbook-hrc.web.app/#/view/rules-on-occupational-safety-and-health-standards/ko/README)"

[__SOURCE](warranty.md)
# Quality Assurance

"[Quality Assurance](https://hrbook-hrc.web.app/#/view/quality-assurance/en/README)"
