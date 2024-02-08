# Safety manual for SafeSpace2.0

{% hint style="warning" %}
The information presented in this manual is the property of Hyundai Robotics.

The manual may neither be copied, in part or in full, nor redistributed without prior written consent from Hyundai Robotics.

It may neither be provided to any third party nor used for any other purposes.



Hyundai Robotics reserves the right to modify this document without prior notification.



**Copyright ⓒ 2020 by Hyundai Robotics Co., Ltd**
{% endhint %}
# About this manual

This manual describes  the safety, installation, use, and maintenance methods of SafeSpace2.0 manufactured by Hyundai Robotics.

Before using the product, read and fully understand the contents of this manual. In addition, keep this manual in an accessible place so that it can be read any time when necessary.

This manual may be provided to customers who purchase products of Hyundai Robotics or may be used as material for internal training programs.

As this manual has been prepared based on standard specifications, it may not apply equally to all models. In addition, the details and specifications of this manual are subject to changes for improving product performance without notice, and Hyundai Robotics will not take responsibility for any consequences of incorrect details, typos, or omissions of this manual. For detailed information on revisions, please visit our website ([www.hyundai-robotics.com](https://www.hyundai-robotics.com)).

Products covered by this manual are :

|     **Item**    |  **Name** | **Version** |
| :-----------: | :-----: | :----: |
|     Teach pendant     |  TP630  |  V1.0  |
|      Controller      |  Hi6a  |  V1.0  |
| Safety control board |  BD642A  |  V04  |
| PROFIsafe communication board |  BD671  |  V2  |
# Copyright

All the programs, files, and contents relating to this product and manual are protected by the Copyright Act and a confidentiality agreement. Any use, reproduction, and disclosure or distribution of this manual to third parties not explicitly permitted by Hyundai Robotics are strictly prohibited.

Copyright ⓒ 2020 HYUNDAI ROBOTICS. All rights reserved.
# Notation Convention

In this manual, the following notation conventions and safety instructions are used to help you understand the contents.

## Description of Figures

Figures are used to help you understand how to operate the product and illustrate what you can see on the screen. For the description of figures, numbers will be marked for the relevant parts, and the corresponding contents will be described as follows.

![](../_assets/image_1_en.png)

## GUI \(Graphical User Interface\)

On the GUI, menu names and button names are enclosed in square brackets \(\[ \]\) and displayed in bold. When you need to select multiple menus in order, mark them with the &gt; symbol between the names.

* Menu with a name: Touch the \[Menu\] button on the initial screen in manual or automatic mode.
* Multiple menus: Touch the \[Set Up\] button &gt; \[5: Initialize &gt; 7: Unit Setting\] menu on the initial screen in manual mode.



## Notation Method for Operation Keys

Keys that are to be pressed on the operation part of the teach pendant to operate functions will be enclosed in single arrow brackets \(&lt; &gt;\) and displayed in bold.

* If you press the &lt;Start&gt; key, the automatic operation of the program created in the robot will start.



## Cross Reference 

This provides the shortcut to the related information in the manual. Cross-references will be in quotation marks and in **bold type**.

* For details of making changes in date and time information, see “**4.5 Date and time setting**.” of “**Operation Manual for Hi6 Controller**” &#x20;

## Note

In this section are some helpful tips or additional information that could be useful when you use the product as follows.

{% hint style="info" %}
When the ![](../_assets/engineer.png)icon blinks in the status bar, it means that you are in engineer mode.
{% endhint %}# Safety precautions

To ensure proper product use and user safety and to prevent property damages, make sure to read and fully understand the following precautions before using the product.

### <mark style="color:green;">Danger</mark>

{% hint style="danger" %}
**\[Danger] impending risk**: If not conformed to, operator deaths or severe injuries may occur.
{% endhint %}

*   Perform a risk assessment on the entire system, not the individual devices. Connecting other devices to the product may increase the risk level of the product or create new risks. If the devices of the integrated robot system have different risk levels, prepare safety devices based on the device with the highest risk level in preparedness for risks.


*   In installing the robot product and other devices, make sure to read, fully understand, and conform to the product installation instructions described in the manual.


*   In case of any issues of the product, such as faults and damages, stop using the product immediately and contact our Customer Support Team.



### <mark style="color:green;">Warning</mark>

{% hint style="warning" %}
**\[Warning] Potential risk**: If not conformed to, operator injuries or property damages, including serious product damages, may occur.
{% endhint %}

*   Take adequate safety measures according to the result of risk assessment, and accurately assign the safe range of robot installation. During the robot operation, product damages or user injuries may occur.


*   Persons who manufacture robot application systems or use the robot must read and fully understand the manual and undergo training in robot operation.


*   For the safety of operators and users, prepare adequate safety facilities such as safety fences before installing the product.


*   Secure sufficient space so that the robot arm can move freely. During the robot operation, product damages or user injuries may occur.

    Fasten locking bolts to the specified torque according to the specification sheet. Loose bolts may lead to damages of the robot because of falling from the installation position.


*   Pay attention to the product connections (power and cables) so that no conductive substances, such as liquid, dust, and metal particles, could infiltrate. Do not poke the connection with sharp objects or apply excessive force during cable connection. Corrosion or temporary short circuits of connectors may lead to product explosion or fires.


*   Check the wiring specification and connect devices with terminals that are suitable for the device types. Make sure to connect safety devices to dedicated terminals because connecting them to general terminals does not guarantee safety functions.


*   Never use damaged cables and do not disconnect cables while the product is in use. Doing so may lead to electric shocks, fires, faults, and injuries.


*   Long-time use of the product may lead to overheating and cause injuries such as burns. In the event it is necessary to touch the product, cool down the product sufficiently by powering it off and leaving it for at least one hour.


*   Never arbitrarily install, modify, disassemble, or repair the product. This may lead to faults and accidents. Hyundai Robotics will not take responsibility for product damages caused by such arbitrary actions.



### <mark style="color:green;">Caution</mark>

{% hint style="warning" %}
**\[Caution] Minor risk**: If not conformed to, minor operator injuries or property damages, including product damages, may occur.
{% endhint %}

*   Do not arbitrarily install, modify, disassemble, or repair the product. It is prohibited for persons other than experts from Hyundai Robotics to modify or attach parts to the product. Product faults caused by it will void free-of-charge services and warranty services.


*   In the event it is necessary to install or repair the product, contact our Customer Support Team to consign the work to experts.


*   Do not install or use the product at a place filled with dust or dirt. Dust or foreign matters may lead to product faults or malfunctions.


*   Do not install or use the product at a place of magnetism, a place which is affected by magnetism, or a place of electromagnetic interferences. Magnetism may lead to product damages or malfunction.


*   In operating the product, do not wear loose clothes or accessories. If you have long hair, you should tie it at the back of your head so it will not entangle between joints and the like of the robot.


*   While the product is in operation, do not enter its operating range or touch the robot. Doing so may lead to injuries.


*   Transport the product as it is packaged to prevent product damages, and store it at a dry and low-humidity place. Storing it at a humid place may lead to product damages or faults caused by moisture infiltration.


*   Store the product at a place that is clean, cool, dry, and free from high variation in temperature and humidity.


*   The product should be moved by two or more persons, and the correct posture should be maintained. If not, the persons may be subject to physical injuries in the waist, arms, legs, and the like.


*   In moving the product using lifting equipment, conform to the local and national safety regulations and the instructions for equipment use.


*   Before moving the product, read and conform to the moving instructions specified in the manual. Hyundai Robotics will not take responsibility for product damages caused during transportation by the customer.


# 1. Safety

# 1.1 Safety requirements

# 1.1.1 Applicable standards

This product has been designed and manufactured in compliance with ISO 10218-1, a safety standard of industrial robots, and ISO/TS 15066, a standard specifying safety requirements for collaborative operation. The safety standards applicable to this product are as follows:

* ISO 10218-1:2011 Robots and robotic devices - Safety requirements for industrial robots - Part 1: Robots
* ISO 10218-2:2011 Robots and robotic devices - Safety requirements for industrial robots - Part 2: Robot systems and integration
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
* IEC 61800-3:2017 Adjustable speed electrical power drive systems - Part 3: EMC requirements and specific test methods
* IEC 61000-6-7:2014 Electromagnetic compatibility (EMC) - Part 6-7: Generic standards - Immunity requirements for equipment intended to perform functions in a safety-related system (functional safety) in industrial locations
* IEC 61326-3-1:2017 Electrical equipment for measurement, control and laboratory use. EMC requirements. Part 3-1: Immunity requirements for safety-related systems and for equipment intended to perform safety-related functions (functional safety) - General industrial applications
# 1.1.2 Safety performance

The safety performance of the emergency stop and external interface(default safety I/O, PROFIsafe) in SafeSpace2.0 is as follows: 
|            **Item**            | **Safety performance** |         **Application standards**         |
| :--------------------------: | :-------: | :-----------------------: |
|              HFT             |     1     | IEC 61508/62061/61800-5-2 |
| SIL (Safety Integrity Level) |     3     | IEC 61508/62061/61800-5-2 |
|           Category           |     4     |        ISO 13849-1        |
|    PL (Performance Level)    |     e     |        ISO 13849-1        |
|    		PFH    			   |  1.5E-08  |         IEC 61508         |


The safety performance of other safety functions is as follows:
|            **Item**            | **Safety performance** |         **Application standards**         |
| :--------------------------: | :-------: | :-----------------------: |
|              HFT             |     1     | IEC 61508/62061/61800-5-2 |
| SIL (Safety Integrity Level) |     2     | IEC 61508/62061/61800-5-2 |
|           Category           |     3     |        ISO 13849-1        |
|    PL (Performance Level)    |     d     |        ISO 13849-1        |
|    		PFH    			   |  1.5E-07  |         IEC 61508         |

# 1.2 Safety measures

This section describes the safety functions embedded into the product and the measures for ensuring the safety of users and operators.
# 1.2.1 Safety functions

SafeSpace2.0 is intended to carry out collaborative tasks based on the following safety functions. For the details of the safety functions, see the "[**3. SafeSpace2.0 Safety functions**](../../3-safety-function/README.md)"

* STO: Safe Torque Off
* SS1: Safe Stop 1
* SS2: Safe Stop 2
* EM Stop, Emergency Stop
* Protective Stop
* Normal stop
* SBC: Safe Brake Control
* Safety Outputs
* Safety Inputs
* PROFIsafe
* SOS: Safe Opertaing Stop
* Joint-SLP, Joint Angle Monitoring
* Joint-SLS, Joint Angular Speed Monitoring
* Collision Detection
* TCP-SLP, TCP Position Monitoring
* TCP Orientation Monitoring
* TCP-SLS, TCP Speed Monitoring
* Momentum Monitoring
* Power Monitoring
# 1.2.2 Safety training

To effectively use the product functions, the user must read and fully understand the manual, and install, use, and maintain the product properly. The product user will be responsible for having the full knowledge of and conforming to the robot-related safety regulations of the locality in which the robot is installed and used, and for the proper designing, installation, and operation of the safety devices that can guarantee the safety of the workers of the robot system.

*   All workers who install, use, and maintain the robot system must read and fully understand the manual. They must be fully knowledgeable of the safety precautions(:warning:).


*   Hyundai Robotics establishes and implements plans to provide training in product installation, use, and maintenance. Product operators and workers must undergo the relevant training programs before handling the product.


* Workers who are responsible for the robot’s teaching and checkups must undergo a training program in robot use and safety before handling the robot. The safety training program covers the following topics:
  *   The concept of safety and the purposes and functions of the safety devices


  *   The procedures for handling the robot safely


  *   The performance and potential risks of the robot and robot system


  *   The materials relating to the application of specific robots


# 1.2.3 Emergency stop

The emergency stop function is actuated in an emergency where a worker or object enters a hazard area. All the emergency stop switches are installed at places easily accessible from outside the safety areas.

When the emergency stop function is actuated, the robot will immediately stop moving in any case.


*   The servo system power of the robot will be cut off, and the motor brake will be actuated.


*   On the teach pendant screen, an emergency stop message will appear.# 1.2.3.1 Emergency stop switches

emergency stop switches are installed at the controller and the teach pendant. In case of an emergency, press the emergency stop switch.
# 1.2.3.2 Connecting to emergency stop devices of external systems

In addition to the emergency stop switches installed by default, it is possible to add external emergency stop devices according to site conditions and applications. For more details, see “[**2. Installation**](../../../2-installation/README.md)” and “[**3.3.3 Safety I/O**](../../../3-safety-function/3-safety-function/3-safety-io/README.md)”

# 1.3 Risk assement

In a system integration including robots, risk assessment is of great importance that most countries specify it as a statutory requirement. Because safety assessments of robot installation vary depending on methods for integrating robots into systems, the risks of robot integrated systems cannot be assessed only by robots alone.

System administrators should carry out a risk assessment on the robot system according to the instructions specified in ISO 12100 and ISO 10218-2. The technical specifications  ISO/TS 15066 may also be referred to.

Perform risk assessment in consideration of the entire processes of the integrated system including robots. The major objectives of risk assessment are as follows:

* Basic setting of robot use and robot teaching
* Problem diagnosis and maintenance
* Normal operation of installed robots



After installing robots and composing the system, a risk assessment must be performed. In risk assessment, the major points to be determined include the adequacy of the safety devices of integrated robot systems and the necessity for additional emergency stop devices or other safety devices.

It is very important to compose robot integrated systems based on the identification of adequate safety devices. Compose robot integrated systems referring to the relevant details of the manual.

For robots, it is possible to set tool center point (TCP) speed, pressure, power, momentum, collision detection, limit values of reduction ratio, and limit values of joint-specific angles, speeds, and torques. In addition, safety functions can be set by using safety-related inputs/outputs (I/Os). For more details for the composition of safety functions, see the “[**3. SafeSpace2.0 safety functions**](../3-safety-function/README.md)”

In the **\[Safety functions]** menu, the safety-related functions of the collaborative robot can be set, including the following:

*   **Force and power limiting**: Limit the force and pressure at which the robot should stop in case of collision between the robot and an operator.


*   **Momentum limiting**: Limit energy and impact load by decreasing the robot’s motion speed in case of collision between the robot and an operator.


*   **Joint and TCP position limiting**: Limit the robot’s motion so that it does not move to body parts such as the user’s neck or head.


*   **TCP and tool posture limiting**: Limit motion to reduce risks relating to specific sections or characteristics of tools and operating parts (e.g., sharp points of tools or objects under operation).


* **Speed limiting**: Limit the speed of the robot to a low speed so that an operator can escape collision with the robot.

In addition, safety-related functions can be composed by installing the robot at a specific location or using safety I/Os.

The major categories of the risk assessment of robot integrated systems include the following:

* Collision severity of robots
* Collision probability of robots
* Collision avoidance probability of robots



In integrating robot systems, if risk factors (e.g., use of tools unintended for collaborative robots) are not sufficiently removed by the robot’s safety functions, additional protective devices shall be installed according to the risk assessment.
# 1.4 Potential risk

In the risk assessment of an integrated robot system, if the assessment result indicates that risk factors are not sufficiently removed only by the robot’s safety functions, additional protective measures must be established.

In establishing additional protective measures, the following should be considered:

*   Finger pinching (entanglement) between the robot base and the installation support during installation


*   Injuries (such as poking and piercing) caused by sharp edges or protruding parts of obstacles or tools in the operating area


*   Injuries caused by collision with the robot (such as bruises, falling, and bone fractures)


*   Injuries caused by obstacles around the robot (such as poking, piercing, and bone fractures)


*   Injuries caused by loose connections


*   Injuries caused by toxic or hazardous substances under work (such as skin damage and breathing disorders)


*   Displacement of objects under work caused by abrupt power shutoffs


*   Erroneous activation of emergency stop switches caused by confusion with those of other equipment


*   Errors caused by arbitrary modification of the Set up of safety functions



Because the types of potential risks vary depending on system compositions, a risk assessment must be carried out before using an integrated robot system.
# 1.5 Validity and responsibilities

The user should conform to the safety requirements specified in the safety laws and regulations of the country and locality in which the robot is installed and used. Responsibilities of suppliers and users of integrated robot systems include but are not limited to the following:

*   Risk assessment of robot integrated systems


*   Addition or removal of safety devices according to the result of risk assessment


*   Checking that robot integrated systems are properly composed, installed, and set


*   Establishment of the methods and instructions for using robot integrated systems and provision of user training


*   Management of safety devices (prohibition of users from arbitrary modification and manipulation of safety devices)


*   Provision of important pieces of information, contact addresses, and others relating to product use and safety


*   Provision of all types of technical documents including manuals



The safety-related content of this manual does not cover all the risk factors and situations that may occur during product use.
# 1.6 Reaction time


*   **Stopping Reaction time**

    When a Safety function violation is triggered, the reaction time until a stop is 9.8 ms. The response time should be taken into account when calculating the robot's stopping time and stopping distance."

*   **PROFIsafe Reaction time**
	
	When an external stop is triggered via PROFIsafe, the reaction time until a stop is 40.8 ms. To obtain the time until the robot completely stop, the communication cycle, as well as the calculated values for the robot's stopping time and stopping distance, need to be added.

****# 2. Installation

# 2.1 Robot system

Industrial robots are “machines that are equipped with manipulation and movement functions based on automatic control for them to perform various works by using programs at an industrial site.” The collaborative robot is a type of industrial robot.

The robot system consists of a manipulator and a controller that controls the manipulator. A teach pendant that is to be used for setting and manually operating the robot system is attached to the controller.

* Robot: Performs various works in industrial sites such as transporting objects, assembling parts, etc.
* Controller: Adjusts the robot’s operation according to the program setting values set through the teach pendant. It can be interoperated with various external equipment or devices through the input/output port of the controller. 
* Teach Pendant: A device that manages the entire robot system. It enables you to teach the robot a specific posture or setup and control the programs.

The following shows an example of the basic configuration of the robot system.

![Basic Configuration of the Vertical Articulated Robot System ](../_assets/image_285.png)


{% hint style="info" %}
For more details on teach pendant, see “[Operation Manual for Hi6 Controllers.](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/english-tp630/1-robot-system/README)”
{% endhint %}
# 2.2 Safety control board

The safety control module is installed and shipped inside the controller in the form of a board, refer to the controller maintenance manual if the board needs to be replaced.# 2.3 Additional safety I/O module(option)

The additional safety I/O module is installed and shipped inside the controller in the form of a board, refer to the controller maintenance manual if the board needs to be replaced.# 2.4 PROFIsafe module(option)

The PROFIsafe option module is installed and shipped inside the controller in the form of a board, refer to the controller maintenance manual if the board needs to be replaced.# 3. SafeSpace2.0 safety functions

# 3.1 Description of terms

### <mark style="color:green;">Robot monitoring functions</mark>&#xD;

These are the functions for monitoring the speed, force and momentum of the robot.

*   **Joint angle monitoring**

    This monitors the position of each axial joint. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.

*   **Joint speed monitoring**

    This monitors the speed of each axial joint. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.
    
*   **Safe operating stop (SOS) monitoring**

    This monitors whether the robot stops without any slips. In cases when the specified value is exceeded, Stop0 will be actuated. 

*   **Tool center point (TCP) position monitoring**

    This monitors whether the safety tool model violates the safety space. In cases when the safety space is intruded into, the safety stop set by the user will be actuated.
    
*   **TCP orientation monitoring**

    This monitors whether the tool orientation is out of the specified range. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.
    
*   **TCP speed monitoring**

    This monitors the speed of the tool tip. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.
    
*   **Power monitoring**

    This monitors the power of the robot. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.
    
*   **Momentum monitoring**

    This monitors the momentum of the robot. In cases when the specified value is exceeded, the safety stop set by the user will be actuated.


*   **Collision detection**

    In cases when the allowable value is exceeded because of an external force applied to the robot, the safety stop set by the user will be actuated.


### <mark style="color:green;">Safety layout</mark>&#xD;

These are the parameters for the safe space and the tool space that form the criteria for monitoring the TCP position and orientation.

*   **Safety space**

    This refers to the working space and the protected space.
*   **Working space**

    This refers to the space in which the robot carries out work. If the tool or the robot’s model goes out of the working space, the safety stop function will be actuated.
*   **Protected space**

    This refers to the space where the operator should be safeguarded from the robot. If the tool or the robot’s model goes out of the protected space, the safety stop function will be actuated.
*   **Safety tool modeling**

    The tool attached to the robot is modeled in spheres and cones to monitor the TCP position and orientation.
*   **Safety robot modeling**

   The robot’s 2nd axis and 3rd axis are modeled in capsule to monitor its distance from the safety space.



### <mark style="color:green;">Safety stop</mark>&#xD;

This is the function that stops the robot if any safety conditions are violated. There are three methods for the safety stop. For more details on the methods, refer to ISO 13850 or IEC 60204-1.

*   **Stop0**

    The power of the motors of all the joint modules will disconnect immediately, and the motors will stop (uncontrolled stop).
*   **Stop1**

    The motors of all the joint modules will decelerate and stop, and the power of the motors will disconnect (controlled stop). The robot will decelerate as it continues to move along the programmed path, and then it will stop. As soon as the robot stops, its power will be disconnected.
*   **Stop2**

    The motors of all the joint modules will decelerate, and the safe operating stop (SOS) will take effect. The power supply status of all the motors will be retained.


If stop 1 and stop are performed, the deceleration process is monitored through the stop time and distance.

*   **Stop time**

    This monitors the time from start deceleration to actual robot stop. If the robot does not stop within the set time, perform Stop 0 to immediately remove power from the motor.
*   **Stop distance**

    This monitors the distance of TCP from start deceleration to actual robot stop. If the robot does not stop within the set time, perform Stop 0 to immediately remove power from the motor.
# 3.2 Collaborative operation mode

ISO 10218-1 and ISO/TS 15066 describe four operating modes so that operators can practice work safety without being exposed to risks. The collaborative operation should meet a least one of these requirements, and a visual display should show that the system is in collaborative operation when it is in operation.
# 3.2.1 Safety-rated monitored stop

When a person enters the working space, the robot operation will stop. Install an external monitoring device, and use it while connected to the safety control module (SCM).

* When an external device is connected to the safety input, the stop modes (Stop0, Stop1, and Stop2) should be set in the safety input/output (I/O) signal setting.
* When a safeguard and an external emergency stop device are connected, the stop modes must meet the requirements of the international or local regulations.

The reference information on the setting of the related functions is as follows:

* For more details on the setting of safety I/O signals, see “[**3.3.3 Safety I/O signals**](../3-safety-function/3-safety-io/README.md)”
* For more details on the setting of safety stop functions, see “[**1.9 Safety Stop Function**](../3-safety-function/1-robot-safety-condition/9-stop-function.md)”
# 3.2.2 Speed and separation monitoring

The robot operates within a specified distance and speed.

In the speed and separation monitoring mode, the driving speed of the robot is controlled in proportion to the distance and the relative speed between the robot and the operator, utilizing sensors that can detect the operator’s position and speed. You can use the deceleration mode for the inputs of the external sensors that detect distance.

The reference information on the use of the speed and separation monitoring mode is as follows:

* For more details on the setting of deceleration mode, see “[**3.3.1.5 Re plan**](../3-safety-function/1-robot-safety-condition/5-re-plan.md)”
* For more details on the setting of safety I/O signals, see “[**3.3.3 Safety I/O signals**](../3-safety-function/3-safety-io/README.md)”
# 3.2.3 Power and force limiting

This limits the impact on the human body in case of a collision. The collision detection function and power, momentum limiting function can limit the impact on the operator in case of a collision between the operator and the robot.

The collision detection function detects collisions according to the set sensitivity (%). You can also restrict the robot’s driving power by setting the electric power (W) and momentum (kg·m/s).

For more details on the setting of the robot’s safety functions, see “[**3.3 Safety functions**](../3-safety-function/README.md)”
# 3.3 Safety functions


The Safety functions of SafeSpace2.0 can be configured through the settings of the safety parameters. It is used as a response to selected risks in risk assessments conducted by operator.

# 3.3.1 Robot monitoring functions

The robot safety parameters consist of limits to monitor the safety function and stopping methods.

Each safety function can be utilized by storing various sets of activation conditions, limit values and methods of stopping in case of violation.  

You can set parameter values in the following menu.

**\[System]** button > **\[4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction]** 
****


The following safety parameters can be set in the robot monitoring menu.

* **Joint position**: This limits the robot’s joint positions so that its axes can move only within the specified ranges.
* **Joint speed**: This limits the robot’s momentum so that its axes cannot move beyond the specified speeds.
* **SOS**: This monitors the robot's stationary state by checking for abnormal movement on each axis after performing stationary 2
* **TCP speed**: This limits the robot's TCP speed so that axes cannot move beyond the specified speeds.
* **Re plan**: This contorls the speed of robot according to external input signal to perform [3.2.2 Speed and separation monitoring](../../2-collaborative-operation-mode/2-speed-separation-monitoring.md) of collaborative operation mode.
* **Power, collision detection**: This limits the force and pressure in case of a collision between the robot and the operator.
* **Momentum**: This limits the energy and impact load in case of a collision between the robot and the operator.


{% hint style="warning" %}
**\[Caution]** : To ensure the safety of personnel and equipment around the robot, operators and users should perform a risk assessment before configuring the robot’s safety function and set the following details according to the assessment result:

* Set passwords and the like so that the safety configuration cannot be modified by unauthorized persons.
* Set safety-related functions and interfaces.
* Check if the settings are correct before running the robot.
* Check if all the safety functions are configured and if the settings conform to the result of the risk assessment.
{% endhint %}

# 3.3.1.1 Joint space monitoring

These parameters are the limit values for monitoring the safety functions relating to the space in which the robot’s joints move. If a monitoring violation occurs, safety stops (Stop0, Stop1, and Stop2) will be actuated immediately.

![An example of joint space setting (S-axis)](../../../_assets/joint_space.png)

You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > Joint space]** menu.

![Window for setting joint space parameters](../../../_assets/joint_space_param.PNG)

|  **Parameter** |                       **Description**                       |  **Default setting value**  |
| :-------: | :------------------------------------------------: | :----------: |
| Type |  <p>Type of space</p><p>(working space/protected space)</p>  | working space |
| Activation | <p>Activation of function</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stop method</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Joint OnOff |   <p>Activation of each joint</p><p>(On/Off)</p>  |  Off |
| Min |   <p>The angle limit value of a joint</p><p>(-360.0 ~ 360.0 (deg))</p>  |  -360.0 |
| Max |   <p>The angle limit value of a joint</p><p>(-360.0 ~ 360.0 (deg))</p>  |  360.0 |

{% hint style="warning" %}
**\[Caution]**: The safety function is monitored based on the set parameters. In configuring a limit, you must consider the stop reaction time and stopping distance. Before running the robot, verification must be performed.
{% endhint %}
 # 3.3.1.2 Joint speed monitoring

These parameters are the limit values for monitoring the safety functions relating to the speed in which the robot’s joints move. If a monitoring violation occurs, safety stops (Stop0, Stop1, and Stop2) will be actuated immediately.

![An example of joint speed setting](../../../_assets/joint_speed.png)

You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > Joint speed]** menu.

![Window for setting joint speed parameters](../../../_assets/joint_speed_param.PNG)

|  **Parameter** |                       **Description**                       |  **Default setting value**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Activation of function</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stop method</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Joint OnOff |   <p>Activation of each joint</p><p>(On/Off)</p>  |  Off |
| speed |   <p>The speed limit value of a joint</p><p>(0 ~ 5000 (mm/s))</p>  |  5000.0 |

{% hint style="warning" %}
**\[Caution]**: The safety function is monitored based on the set parameters. In configuring a limit, you must consider the stop reaction time and stopping distance. Before running the robot, verification must be performed.
{% endhint %}
 
# 1.6.2 SOS monitoring

SOS monitoring is a function that monitors for abnormal movement of each axis during robot stop operation. If a monitoring violation occurs, Stop0 will be actuated immediately.


You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > Joint SOS]** menu.

![Window for setting joint SOS parameters](../../../_assets/joint_sos_param.PNG)

|  **Parameter** |                       **Description**                       |  **Default setting value**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Activation of function</p><p>(Off/On/Safety Input)</p> |   Off  |
| Joint OnOff |   <p>Activation of each joint</p><p>(On/Off)</p>  |  Off |
| tolerance |   <p>The angle limit value of a joint</p><p>(0.0 ~ 3.0 (deg))</p>  |  0.1 |

{% hint style="warning" %}
**\[Caution]**: Make sure that the robot moves normally before restarting operation if SOS monitoirng is violated.  
{% endhint %}# 3.3.1.4 TCP speed monitoring

This function monitors the TCP speed based on the robot coordinate system. If a monitoring violation occurs, safety stops (Stop0, Stop1, and Stop2) will be actuated immediately.

You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > TCP speed]** menu.

![Window for setting TCP speed parameters](../../../_assets/tcp_speed_param.PNG)

| **Parameter** | 　　　　　　　　　**Description**                                                  |  **Default setting value** |
| :------: | ---------------------------------------------------------------- | :---------: |
| Activation | <p>Activation of TCP speed monitoring function</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stop method</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Replan |   <p>Activation of RePlan function</p><p>(On/Off)</p>  |  Off |
| Limit |   <p>TCP speed limit</p><p>(0 ~ 50000 (mm/s))</p>  | 50000 |
| Rate |   <p>Deceleration ratio for Replan</p><p>(0 ~ 100 (%))</p>  | 0 |
| Delay time |   <p>Monitor changed speed limit after delay time due to RePlan</p><p>(0 ~ 1000(ms))</p>  | 0 |
| Input signal setting |   <p> Input signal assignment for replan</p><p>(0 ~ 16)</p>  |  0 |

{% hint style="warning" %}
**\[Caution]**: The safety function is monitored based on the set parameters. In configuring a limit, you must consider the stop reaction time and stopping distance. Before running the robot, verification must be performed.
{% endhint %}
 # 3.3.1.5 Re plan

Replan is a function that adjusts the speed of the robot based on a input signal from an external safety sensor. The robot's operating speed is changed at a deceleration rate corresponding to the input signal, and the TCP speed is monitored at a speed corresponding to the delay time. If the delay time is insufficient or the robot is not decelerated enough to violate the TCP speed limit, the safety stop (Stop0, Stop1, Stop2) will be activated immediately.

You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > Re plan]** menu.

![Window for setting raplan parameters](../../../_assets/replan.PNG)

|  **Parameter** |                       **Description**                       |  **Default setting value**  |
| :-------: | :------------------------------------------------: | :----------: |
| Replan |   <p>Activation of RePlan function</p><p>(On/Off)</p>  |  Off |
| Limit |   <p>TCP speed limit</p><p>(0 ~ 50000 (mm/s))</p>  | 50000 |
| Rate |   <p>Deceleration ratio for Replan</p><p>(0 ~ 100 (%))</p>  | 0 |
| Delay time |   <p>Monitor changed speed limit after delay time due to RePlan</p><p>(0 ~ 1000(ms))</p>  | 0 |
| Input signal setting |   <p> Input signal assignment for replan</p><p>(0 ~ 16)</p>  |  0 |

{% hint style="warning" %}
* In configuring a speed limit, you must consider the stop reaction time and put a cover on the target to prevent collisions and injuries.
* Because the speed increases in proportion to kinetic energy and a high payload may increase the robot’s momentum, the collision of the robot with an external object may generate significant impact. In the collaborative operation space, operate the robot while maintaining a safe speed and payload.
{% endhint %}
# 3.3.1.6 Collision detection

If the external force applied to the robot exceeds the allowable value, it is recognized as a collision. The sensitivity of each axis can be adjusted. If the sensitivity is higher, the smaller the external force will be recognized as a collision. If a monitoring violation occurs, safety stops (Stop0, Stop1, and Stop2) will be actuated immediately.

You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > Collision detection]** menu.

![Window for setting collision detection parameters](../../../_assets/col_det.PNG)

| **Parameter** | 　　　　　　　　　**Description**                                                  |  **Default setting value** |
| :------: | ---------------------------------------------------------------- | :---------: |
| Activation | <p>Activation of function</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stop method</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Joint OnOff |   <p>Activation of each joint</p><p>(On/Off)</p>  |  Off |
| Sensitivity |   <p>The sensitivity of the collision detection function</p><p>(0 ~ 200 (%))</p>  |  100 |

{% hint style="warning" %}
* Because the speed increases in proportion to kinetic energy and a high payload may increase the robot’s momentum, the collision of the robot with an external object may generate significant impact. In the collaborative operation space, operate the robot while maintaining a safe speed and payload.
* If the tool and additional load information are set differently from the actual one, error detection would be occured incorrectly. Please check the information before using the function.
{% endhint %}
# 3.3.1.7 Power monitoring

It is a function that monitors whether the robot's power exceeds the allowable value. If a monitoring violation occurs, safety stops (Stop0, Stop1, and Stop2) will be actuated immediately.

You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > Power]** menu.

![Window for setting power monitoring parameters](../../../_assets/power.PNG)

| **Parameter** | 　　　　　　　　　**Description**                                                  |  **Default setting value** |
| :------: | ---------------------------------------------------------------- | :---------: |
| Activation | <p>Activation of function</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stop method</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Power |   <p>The power limit of robot</p><p>(80 ~ 1000 (W))</p>  | 1000 |

{% hint style="warning" %}
* Because the speed increases in proportion to kinetic energy and a high payload may increase the robot’s momentum, the collision of the robot with an external object may generate significant impact. In the collaborative operation space, operate the robot while maintaining a safe speed and payload.
* If the tool and additional load information are set differently from the actual one, error detection would be occured incorrectly. Please check the information before using the function.
{% endhint %}
# 3.3.1.8 Momentum monitoring

It is a function that monitors whether the robot's momentum exceeds the allowable value. If a monitoring violation occurs, safety stops (Stop0, Stop1, and Stop2) will be actuated immediately.

You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > Momentum]** menu.

![Window for setting momentum monitoring parameters](../../../_assets/momentum.PNG)

| **Parameter** | 　　　　　　　　　**Description**                                                  |  **Default setting value** |
| :------: | ---------------------------------------------------------------- | :---------: |
| Activation | <p>Activation of function</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stop method</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Momentum |   <p>The momentum limit of robot</p><p>(5 ~ 3000 (kg m/s))</p>  | 1000 |

{% hint style="warning" %}
* Because the speed increases in proportion to kinetic energy and a high payload may increase the robot’s momentum, the collision of the robot with an external object may generate significant impact. In the collaborative operation space, operate the robot while maintaining a safe speed and payload.
* If the tool and additional load information are set differently from the actual one, error detection would be occured incorrectly. Please check the information before using the function.
{% endhint %}
# 3.3.1.9 Safety Stop

Set an adequate safety stop type for each safety stop function. The safety stop functions, which stop the robot under a safe condition in case of a safety violation, include the following three types. All types of safety stop functions meet the requirements of Clause 4.2.2.4 of IEC 61800-5-2.

* **Stop0**: The power of the motors of all the joint modules will disconnect immediately, and the motors will stop.
* **Stop1**: The power of the motors of all the joint modules will decelerate, and the motors will stop. Then, the power of the motors will be disconnected.
* **Stop2**: The motors of all the joint modules will decelerate, and the safe operating stop (SOS) function will take effect. The power supply status of all the motors will be retained.

The stop type due to a safety function violation is set in the parameter setting menu for each function.
The stop type settings for stops required by ISO 10218-1 are as follows.

You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > Safety stop]** menu.

![](../../../_assets/safety_stop.PNG)

|  **Parameter** |                       **Description**                       |  **Default setting value**  |
| :-------: | :------------------------------------------------: | :----------: |
| EM stop |  <p>Emergency stop</p><p>(Stop 0, Stop 1)</p>  | Stop 0 |
| Protective stop | <p>Protective stop</p><p>(Stop 0, Stop 1, Stop 2)</p> |   Stop 0 |
| Normal stop |   <p>Normal stop</p><p>(Stop 0, Stop 1)</p>  | Stop 0 |
| Manual stop |   <p>Speed violation stop in manual mode</p><p>(Stop 0, Stop 1)</p>  |  Stop 0 |


{% hint style="warning" %}
**\[Caution]**: You should set an adequate stopping method for each function based on the result of the risk assessment.
{% endhint %}
# 3.3.2 Safety layout

This sets the safety space, safety tools and safety robot links to monitor robot's position and orientation.
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
{% endhint %}# 3.3.2.4 TCP orientation monitoring

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
# 3.3.3 Safety I/O# 3.3.3.1 Default Safety I/O

Set the parameters of Default Safety I/O.
There are 4 input signals and 1 output signal, all of which are dual signals.

**1. Default Safety Input**

![Default Input Image](../../../_assets/safetyio_profisafe/default_in.PNG)

 - Pulse Test : You can select whether to use Pulse Test for each channel.
 - Error Latch Time : If an error occurs in a channel, even if the error is recovered, the Fail-Safe value is changed to the currently input signal after the **Error Latch time**.(Unit : msec)
 - Filter Time : For each channel, a consistent signal must be input during the **Filter Time** to be processed as a valid signal. (Unit: msec)
 - Discrete Time : Default Safety Input is treated as a valid signal when two dual signals have the same value, and if these two signals differ for a time greater than the **Discrete time** , an alarm is generated. (Unit : msec)
 
**2. Safety Output**

![Default Output Image](../../../_assets/safetyio_profisafe/default_out.PNG)

 - Pulse Test : You can select whether to use Pulse Test for each channel.
 - Error Latch Time : If an error occurs in a channel, even if the error is recovered, the Valid output signal is produced from the Fail-Safe value after the **Error Latch Time** has elapsed. (Unit: msec)


# 3.3.3.2 Additional Safety I/O

Set parameters of Additional Safety I/O.
There are 8 input signals and 4 output signals, and they all operate as dual signals.

**1. Additional Safety Input/Output**

![Additional Input Image](../../../_assets/safetyio_profisafe/add_io.PNG)

 - Enable : Determines whether to use Additional Safety I/O
 - Filter time : For each channel, a consistent signal must be input during the **Filter Time** to be processed as a valid signal. (Unit: msec)
 - Discrete time : Additional Safety Input is treated as a valid signal when two dual signals have the same value, and if these two signals differ for a time greater than the **Discrete time** , an alarm is generated. (Unit : msec)
 - Input Error Latch time :If an error occurs in a channel, even if the error is recovered, the Fail-Safe value is changed to the currently input signal after the **Error Latch time**.(Unit : msec)
 - Output Error Latch time : If an error occurs in a channel, even if the error is recovered, the Valid output signal is produced from the Fail-Safe value after the **Error Latch Time** has elapsed. (Unit: msec)
 
 

# 3.3.3.3 Linker

Linker serves to connect external signals such as Default Safety I/O, Additional Safety IO, and PROFIsafe I/O with various logical signals or state variables of the robot controller.

![Additional Input Image](../../../_assets/safetyio_profisafe/linker.PNG)

- I/O Linker Add : To set up the linker, select the desired function from the I/O function list on the left, press the **[+]** button, and select Index (H/W ch or Bit number). According to I/O function list You can select detailed channels by selecting Subset.

- I/O Linker Delete : Linker settings can be deleted by selecting a linker setting on the right side of the screen and pressing the **[-]** button above.

![Additional Input Image](../../../_assets/safetyio_profisafe/linker_add.PNG)
 


﻿
# 3.3.3.4 PROFINET

**1. PROFINET HW(BD671)**
![Profinet Consol Image](../../../_assets/safetyio_profisafe/BD671_hw.PNG)

- Power Input : 24Vdc input
- Serial Communication Port : Connect Cable with BD642A Board
- PROFINET I/O Ethernet Port : Connect with PROFINET Master
- F/W Download Port : F/W download via J Link
- RS232 Port 
	- Baudrate : 115200 bps
	- Data : 8bit, Parity : none, Stop bits : 1bit
- LED
	- LED1 : Maintenance LED
	- LED2 :  Diagnosis LED
	- LED3 :  Run LED
	- LED4 :  Error LED
	- DCP ( LED3, LED4 Blinking)


**2. Profinet settings**

PROFINET settings can be changed through RS232 communication of BD671. 
In this chapter, PROFINET and the related parameters are explained.

![Profinet Consol Image](../../../_assets/safetyio_profisafe/BD671_console.png)

 - S : Add Sub Module.
 - s : Removes a SubModule.
 - H : Shows a list of currently installed submodules.
 - n : Set the name of the PROFINET
 - N : Set the MAC address of the PROFINET device.
 - o : Set the IP address, Subnet mask, and Gateway.

**3. Moudule information**
 - Module
	 - ID : 0x21
	 - Sub Module ID : 0x2
	 - Description :  8 Bytes I/O PS2v61
	 - Input data Size : 13 Bytes
	 - Output data Size : 13 Bytes
	 - Allowed slot : 1
	 - Allowed subslot :  1

**4. Spec**
	- PNIO Version : V2.43
	- Conformance Class : B
	- Application Class : Functional Safety
	- Net load Class : II
	- MRP (Media Redundancy Protocol)
	- Device Redundancy (S2)
	- Dynamic Reconfiguration (DR)
	- I&M Records 0 ~ 4
	- Supported Protocols : SNMP, LLDP
	- Minimum Device Interval : 1 ms
	- iParameter : Not supported.
	- Parameterization in Run : Not supported.
	- PROFIenergy : Not supported.	 

> Parameter settings using the TP below are in preparation.

![Profinet TP Image](../../../_assets/safetyio_profisafe/profinet.PNG)

 - PROFINET IO Device Name : Set the name of the PROFINET device. The first letters of the device's name are fixed as "HRC-PN-DEV-" and the user can choose the numbers that follow.
 - IP address : Set the IP address. ex) 192.168.1.100
 - Subnet mask : Set the subnet mask. ex)255.255.255.0
 - Gateway : Set the gateway address. ex)192.168.1.1
 - MAC address : This parameter cannot be set and can only be read.

# 3.3.3.5 PROFIsafe

 **1. PROFIsafe settings**

![Profisafe Consol Image](../../../_assets/safetyio_profisafe/BD671_console.png)

 - Source Address : Set the source Address. (fixed to 1)
 - Destination Address : Set the destination Address. (Setting range : 1 ~ 65534)
 
  **2. Notes** 
  
 - Address Type :  Address Type 1 (Check Destination Address only)
 - Reaction on Device_Fault : When this device enters a Fault state, all F-Output will be changed to Fail-safe (0) status. After resolving the device's Fault state, a process of reintegrating the F-Device is necessary from the F-Host using commands such as Global Acknowledge.
 
 **3. Alarm List** 

|Alarm No.|Alarm Decsription  | 
|--|--|
| 0x10 |Parameter setting error |
| 0x13 |Communication error|
| 0x19 |Safety function error |
| 0x1C |Internal communication error 1 |
| 0x1D |Internal communication error 2 |
| 0x1E |Internal communication error 3 |
| 0x40 |F-Dest Address setting error |
| 0x41 |F-Dest Address value is invalid |
| 0x42 |F-Src Address setting error |
| 0x43 |F-Watchdog value is invalid
| 0x45 |F-CRC length is invalid |
| 0x46 |F-PAR version is invalid |
| 0x47 |CRC1 is invalid |
| 0x4C |F-Block ID is invalid |
| 0x4D |CRC2 is invalid|
| 0x4E |F-Watchdog timeout|


> Parameter settings using the TP below are in preparation.

![Profisafe TP Image](../../../_assets/safetyio_profisafe/profisafe.PNG)

 - Source Address : Set the source Address. (fixed to 1)
 - Destination Address : Set the destination Address. (Setting range : 1 ~ 65534)
# 4. Configuration of safety functions

# 4.1 Check before setting the safety functions

# 4.1.1 Encoder offset

The accuracy of encoder data is important because the safety functions detect the robot’s position and speed based on the data transmitted by the encoders attached to the axes. Therefore, before using the safety functions, check whether the encoder values match the actual values.

1\. Check the zero mark of each axis of the robot and move the axes.


Move each axis with the jog if a stop occurs because of a safety function violation. For more details on recovery, see “[**6.1 Recovery**](../../6-recovery/README.md)”.

2\. In the pose information window on the workspace, check whether the axial coordinate values of the robot are displayed at the reference pose(**0, 90, 0, 0, 0, 0** \[deg]).


* Click the **\[+]** button at the top right part of the panel stack if the pose information window does not appear on the workspace. Then, click **\[Pose]** in the panel selection wind


3\. Proceed to the next step if the difference of the angular value is no larger than 0.01. Otherwise, carry out the encoder offset if it is larger than 0.01.

4\. Reboot the system.

{% hint style="info" %}
For more details on the encoder offset, see “[7.4.4 Encoder offsets](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/english-tp630/7-system/4-robot-parameter/4-encoder-offset/README)” of the “[Operation Manual for Hi6 Controllers.](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/english-tp630/README)”
{% endhint %}
# 4.1.2 Setting of tool data

The safety functions monitor the entire robot system including the tool attached to the robot’s tool flange. Therefore, the smaller the difference between the tool data and its actual value, the more accurately the safety functions will work. Set the length and angle of the tool based on the flange coordinate system and input the information on the weight, center of gravity, and inertia of the tool in the applicable units.

1. Set the operating mode to the manual mode.
2. Disconnect the power of the motor by pressing the emergency stop button.
3. Select the **\[Configure]** > **\[3: Robot parameter > 1: Tool data]** menu.
4. Check the data of each axis, set the weight, center of gravity, and inertia of the tool, and save the values by clicking the **\[OK]** button.

![](../../_assets/image20.jpeg)

* To easily create new tool data from scratch utilizing the current program, click the \[Auto calibration] button.
* To correct the tool angle, click the \[Angle calibration] button.
* To add a new user coordinate system or delete one, use the \[+] or \[-] buttons, respectively.
* To view and edit the detailed information of tool data, select a tool data name to be viewed and edited.
* To copy the information on tool data and paste it to that of another, use the \[Copy page] and \[Paste page] buttons, respectively.

{% hint style="info" %}
* When there is no information on the weight and center of gravity of a tool, you can estimate the values using the load estimation function.
* For more details on tool data setting, see “[**Operation Manual for Hi6 Controllers.**](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/english-tp630/7-system/4-robot-parameter/1-tool-data/README)”
{% endhint %}
# 4.1.3 Setting of password

The parameters of the safety function must be set and managed by the designated person in charge. Users designated as administrators are given administrator privileges and passwords to set up the system. The password for setting up the system is mandatory when setting safety function parameters, and if the password is incorrect, it cannot be set by changing the parameters.

1. Push the **\[System]** button and enter the > **\[5: Initialize > 11: System password setting]** menu. The password setting window will pop up.
2. After enter the password, touch the **\[OK]** button.

![](../../_assets/4/4-1-3-1.png)

* When setting the parameters of the safety function, you must enter the system setup password to save the changes.

{% hint style="warning" %}
* It is recommended that the password be set to at least 4 characters.
* If you lose your password, contact your engineer.
{% endhint %}
# 4.1.4 Certification

Safety parameters are protected by the certificate; for the security of the stored safety parameters, you must first issue a certificate. A system password is required to verify, delete, and issue authentication status.

1. **\[System]** button > **\[4: Application parameter > 18: SafeSpace2.0 > Certificate file]**

![](../../_assets/4/4-1-4-1.png)

* Verify certificate status
  Touch the **\[Confirmation]** button.
  Enter the system password.
  check the result.

* Issue certificate file
  Touch the **\[Issue]** button.
  Enter the system password.
  check the result.

* Discard certificate file
  Touch the **\[Discard]** button.
  Enter the system password.
  check the result.
# 4.2 Change safety parameter

Modify the safety parameter values and apply them to the system. Values that have not been applied will be initialized when the setting screen changes.

1. **\[System]** button > **\[4: Application parameter > 18: SafeSpace2.0 > Parameter setup]**, touch the menu.

![](../_assets/4/4-1-5-1.png)

2. Press the page button to navigate to the page where you want to change the parameters. If you do not touch the **\[OK]** button, the changed parameters will be initialized when you move to another page.
3. Modify the parameter values and touch the **\[OK]** button, which temporarily saves the parameters on the page.

* Check the modified values on the page and touch the **\[Appky all]** button.

![](../_assets/4/4-1-5-2.png)

* Pages not pressed **\[OK]** button will not reflected. Please check the message and proceed.

* Enter **\[System password]** to verify the results.

![](../_assets/4/4-1-5-3.png) ![](../_assets/4/4-1-5-4.png)# 5. Safety status monitoring

This monitors safety function violations and the status of the SCM(SCM: Safety Control Module) board. You can view the statuses of the robot limiting functions, joint limiting functions, and the SCM board. 

You can check in **\[System > 4: Application parameter > 18: SafeSpace2.0 > Monitoring]** menu.# 5.1 Robot monitoring function status

You can check robot monitoring function status in **\[System > 4: Application parameter > 18: SafeSpace2.0 > Monitoring] > [Robot monitoring status]** menu.

![Safety status of robot](../_assets/mon_robot.PNG)


* Check the robot monitoring function status
  * **\[TCP position]**: TCP position monitoring violations
  * **\[TCP speed]**: TCP speed monitoring violations
  * **\[TCP orient]**: TCP orientation monitoring violations
  * **\[Power]**: Power monitoring violations
  * **\[Momentum]**: Momentum monitoring violations
  * **\[Collision]**: Collision detectionmonitoring violations
  * **\[SOS]**: SOS(Safe Operating Stop) monitoring violations
  * **\[Joint speed]**: Joint speed monitoring violations
  * **\[Joint position]**: Joint position monitoring violations
  
# 5.2 Safety I/O status monitoring

You can check the safety I/O status in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Monitoring]** menu.

![Safety I/O](../_assets/mon_safetyio.PNG)


# 6. Recovery

 In manual mode, you can clear errors that occur because of the safety function violations during monitoring. Because position detection is disabled in manual mode, you can drive the robot and adjust its angle and position without violating the safety functions.


{% hint style="warning" %}
**\[Caution]**: After clearing the violation, recheck the safety layout setting and the teaching position of the operating program.
{% endhint %}
# 6.1	Recovery in case of robot position violations

Robot position violations are situations in which the robot’s position exceeds a safety space, and these include TCP position, TCP orientation, and joint monitoring violations. When a robot position violation occurs, you can only clear the error by moving the robot’s physical position.

1.  Change the mode switch to manual mode.


2.  Turn on the motor by using the enabling switch on the teach pendant.


3.  Use the teaching device to move the robot back to a safety space.


4.  On the safety condition monitoring window, check if the status of each space is displayed as **SAFE**.


{% hint style="warning" %}
**\[Caution]**: After clearing the violation, recheck the safety layout setting and the teaching position of the operating program.
{% endhint %}
# 6.2	Recovery in case of robot speed violations

Robot speed violations are situations in which the robot’s speed exceeds a safety limit, and these include TCP speed, joint speed, power, and momentum monitoring violations. Because the robot detects the instantaneous speed in the case of robot speed violations, you can clear the error without moving the robot’s position.

1.  Change the mode switch to manual mode.


2.  On the safety condition monitoring window, check if the status of each space is displayed as **SAFE**.


{% hint style="warning" %}
**[Caution]**

* After clearing the violation, make sure to recheck all speed-related safety parameters and the speed displayed on the operating program.
{% endhint %}
# 6.3	Recovery in case of robot force violations

Robot force violations are situations in which external force is applied on the robot or in which the amount of the force used by the robot internally exceeds a safety limit, and these include collision detection, power, and momentum monitoring violations. You can clear errors depending on the causes of the violations.


1.  Remove the external factor that is applying force on the robot.


2.  Change the mode switch to manual mode.


3.  On the safety condition monitoring window, check if the status of each space is displayed as **SAFE**.


{% hint style="warning" %}
**[Caution]**

* After clearing the violation, recheck safety function setting, tool data, the teaching position and speed of the operating program.
{% endhint %}
# 6.4	Recovery in cases of safe operating stop (SOS) violations

SOS violations are situations in which the robot’s motion is detected while its motor is on and is supposed to be in a stop state. Because the robot detects the instantaneous speed in the case of robot speed violations, you can clear the error without moving the robot’s position.

1.  Change the mode switch to manual mode.


2.  Remove the external factor that is applying force on the robot.


3.  On the safety condition monitoring window, check if the status of each space is displayed as **SAFE**.


{% hint style="warning" %}
**[Caution]**

* After clearing the violation, recheck the SOS parameters.
* Turn on the motor in the automatic mode and check if the error does not persist.
* If the same error recurs, check the motor and reducer of the pertaining axis.
{% endhint %}
# 7. Error messages

The safety function error messages of SafeSpace2.0 are as follows:
# 7.1 Error List

| **Code** |                  **Message**                  |                            **Cause**                           | 　　　　**Solutions**                                                                                                                                  |
| :----: | :---------------------------------------: | :---------------------------------------------------------: | -------------------------------------------------------------------------------------------------------------------------------------------- |
|SE101|The received safety configuration file has been corrupted|The received CRC32 data does not match the original value|<ul><li>Replace the safety board with a new one.</li><li>Please contact the maintenance department of this company if the same error occurs again even after replacing the safety board.</li></ul>|
|SE201|<p>The Response of safety board has been delayed</p>|Safety communication(FSoE) encountered a response delay error|<ul><li>Replace the safety board with a new one.</li><li>Please contact the maintenance department of this company if the same error occurs again even after replacing the safety board.</li></ul>|
|SE202|<p>Data corruption error of safety communication(FSoE)</p>|CRC data received in the safety communication module does not match original value|<ul><li>Replace the safety board with a new one.</li><li>Please contact the maintenance department of this company if the same error occurs again even after replacing the safety board.</li></ul>|
|SE301|<p>The internal communication error (CPU1-CM) in the safety board</p>|Internal IPC communication data CRC error between CPU1 and CM|<ul><li>Replace the safety board with a new one.</li><li>Please contact the maintenance department of this company if the same error occurs again even after replacing the safety board.</li></ul>|
|SE302|<p>The internal communication error(FSI) in the safety board</p>|FSI communication CRC error occured between MCUs in the safety board|<ul><li>Replace the safety board with a new one.</li><li>Please contact the maintenance department of this company if the same error occurs again even after replacing the safety board."
|SE303|<p>The internal communication(FSI) delay error</p>|The Communication dealy occured between MCUs in the safety board|<ul><li>Replace the safety board with a new one.</li><li>Please contact the maintenance department of this company if the same error occurs again even after replacing the safety board.</li></ul>|
|SE304|<p>The received file through the internal communication(FSI) has been corrupted</p>|The recevied CRC value does not match the original value|<ul><li>Replace the safety board with a new one.</li><li>Please contact the maintenance department of this company if the same error occurs again even after replacing the safety board.</li></ul>|
|SE401|<p>The data corruption error occured between CPU1-CPU2 in the safety board</p>|Internal CPU1-CPU2 IPC communication data CRC error|<ul><li>Replace the safety board with a new one.</li><li>Please contact the maintenance department of this company if the same error occurs again even after replacing the safety board.</li></ul>|
|SE402|<p>The delay error occured between CPU1-CPU2 in the safety board</p>|The Communication(IPC) dealy occured between CPU1 and CPU2 in the safety board|<ul><li>Replace the safety board with a new one.</li><li>Please contact the maintenance department of this company if the same error occurs again even after replacing the safety board.</li></ul>|
|SE403|<p>The data corruption error occured between CPU2-CPU2 in the safety board</p>|The recevied CRC data does not match the original value during performing SCI communication|<ul><li>Replace the safety board with a new one.</li><li>Please contact the maintenance department of this company if the same error occurs again even after replacing the safety board.</li></ul>|
|SE404|<p>The delay error occured between CPU2-CPU2 in the safety board</p>|Communication delay occured during performing SCI communication|<ul><li>Replace the safety board with a new one.</li><li>Please contact the maintenance department of this company if the same error occurs again even after replacing the safety board.</li></ul>|
|SE601|<p>Safe parameter range exceeded(General setup)</p>|The parameter set in the General setup configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the General setup configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE602|<p>Safe parameter range exceeded(Joint space)</p>|The parameter set in the Joint space configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Joint space configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE603|<p>Safe parameter range exceeded(Joint speed)</p>|The parameter set in the Joint speed configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Joint speed configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE604|<p>Safe parameter range exceeded(SOS)</p>|The parameter set in the SOS configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the SOS configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE605|<p>Safe parameter range exceeded(TCP speed)</p>|The parameter set in the TCP speed configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the TCP speed configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE606|<p>Safe parameter range exceeded(Cell ares)</p>|The parameter set in the Cell area configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Cell area configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE607|<p>Safe parameter range exceeded(Tool model)</p>|The parameter set in the Tool model configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Tool model configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE608|<p>Safe parameter range exceeded(Robot model)</p>|The parameter set in the Robot model configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Robot model configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE609|<p>Safe parameter range exceeded(Self collision)</p>|The parameter set in the Self collision configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Self collision configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE610|<p>Safe parameter range exceeded(TCP orientation)</p>|The parameter set in the TCP orientation configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the TCP orientation configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE611|<p>Safe parameter range exceeded(Replan)</p>|The parameter set in the Replan configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Replan configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE612|<p>Safe parameter range exceeded(Power)</p>|The parameter set in the Power configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Power configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE613|<p>Safe parameter range exceeded(Momentum)</p>|The parameter set in the Momentum configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Momentum configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE614|<p>Safe parameter range exceeded(Collision detection)</p>|The parameter set in the Collision detection configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Collision detection configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE615|<p>Safe parameter range exceeded(Safe stop)</p>|The parameter set in the Safe stop configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Safe stop configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE616|<p>Safe parameter range exceeded(PROFINET)</p>|The parameter set in the PROFINET configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the PROFINET configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE617|<p>Safe parameter range exceeded(PROFIsafe)</p>|The parameter set in the PROFIsafe configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the PROFIsafe configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE618|<p>Safe parameter range exceeded(Safety IO)</p>|The parameter set in the Safety IO configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Safety IO configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE619|<p>Safe parameter range exceeded(Add Safety IO)</p>|The parameter set in the Add Safety IO configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Add Safety IO configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE620|<p>Safe parameter range exceeded(IO Function Setting)</p>|The parameter set in the IO Function Setting configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the IO Function Setting configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE621|<p>Safe parameter range exceeded(Additional load)</p>|The parameter set in the Additional load configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Additional load configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE622|<p>Safe parameter range exceeded(Tool info)</p>|The parameter set in the Tool info configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Tool info configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE623|<p>Safe parameter range exceeded(Maintenance)</p>|The parameter set in the Maintenance configuration menu has exceeded the range.|<ul><li>Please check that the parameters set in the Maintenance configuration menu do not exceed the range.</li><li> Perform a safe parameter initialization.</li><li>Replace the safety board.</li></ul>|
|SE1301|<p>MCUA HW-BIST Diagnostic error</p>|CPU,FPU of CPU1 are abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1302|<p>MCUA PIE_RAM Diagnostic error</p>|Address of cpu1 PIE Vector handler mismatch.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1303|<p>MCUA CPU register Diagnostic error</p>|CPU1 Core Register read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1304|<p>MCUA FPU register Diagnostic error</p>|CPU1 FPU Register read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1305|<p>MCUA VCRC register Diagnostic error</p>|CPU1 VCRC Register read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1306|<p>MCUA march ram Diagnostic error</p>|CPU1 ram read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1307|<p>MCUA march ram Diagnostic error</p>|CPU1 ram copy area read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1308|<p>MCUA FLASH crc Diagnostic error</p>|CPU1 Flash crc value is inconsistent.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1309|<p>MCUA oscillator Diagnostic error</p>|CPU1 external oscillator is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1310|<p>MCUA CM timeout error</p>|CM operation is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1311|<p>MCUA CPU2 timeout error</p>|CPU2 operation is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1312|<p>MCUA CPU1 timeout error</p>|CPU1 CM operation is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1313|<p>MCUA boot flash CRC error</p>|CPU1 boot Flash crc value is inconsistent.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the CPU1 executable.</li></ul>|
|SE1314|<p>MCUA boot RAM CRC error</p>|CPU1 boot ram crc value is inconsistent.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the CPU1 executable.</li></ul>|
|SE1316|<p>MCUA PIE_RAM Diagnostic error</p>|Address of cpu2 PIE Vector handler mismatch.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1317|<p>MCUA CPU2 register Diagnostic error</p>|CPU2 Core Register read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1318|<p>MCUA FPU register Diagnostic error</p>|CPU2 FPU Register read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1319|<p>MCUA VCRC register Diagnostic error</p>|CPU2 VCRC Register read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1320|<p>MCUA march ram Diagnostic error</p>|CPU2 ram read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1321|<p>MCUA flash crc Diagnostic error</p>|CPU2 Flash crc value is inconsistent.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1322|<p>MCUA boot flash CRC error</p>|CPU2 boot Flash crc value is inconsistent.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the CPU2 executable.</li></ul>|
|SE1323|<p>MCUA Temperature limit error</p>|The temperature of the SCM board is too high.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1324|<p>MCUA Voltage limit error</p>|The voltage supply on the SCM board is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1325|<p>MCUB HW-BIST Diagnostic error</p>|CPU,FPU of CPU1 are abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1326|<p>MCUB PIE_RAM Diagnostic error</p>|Address of cpu1 PIE Vector handler mismatch.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1327|<p>MCUB CPU register Diagnostic error</p>|CPU1 Core Register read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1328|<p>MCUB FPU register Diagnostic error</p>|CPU1 FPU Register read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1329|<p>MCUB VCRC register Diagnostic error</p>|CPU1 VCRC Register read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1330|<p>MCUB march ram Diagnostic error</p>|CPU1 ram read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1331|<p>MCUB march ram Diagnostic error</p>|CPU1 ram copy area read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1332|<p>MCUB flash crc Diagnostic error</p>|CPU1 Flash crc value is inconsistent.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1334|<p>MCUB oscillator Diagnostic error</p>|CPU1 external oscillator is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1335|<p>MCUB CM timeout error</p>|CM CM operation is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1336|<p>MCUB CPU2 timeout error</p>|CPU2 CM operation is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1337|<p>MCUB boot flash CRC error</p>|CPU1 Flash crc value is inconsistent.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the CPU1 executable.</li></ul>|
|SE1338|<p>MCUB boot RAM CRC error</p>|CPU1 boot ram crc value is inconsistent.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the CPU1 executable.</li></ul>|
|SE1339|<p>MCUB PIE_RAM Diagnostic error</p>|cpu2 PIE Vector handler address mismatch.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1345|<p>MCUB CPU register Diagnostic error</p>|Address of cpu2 PIE Vector handler mismatch.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1346|<p>MCUB FPU register Diagnostic error</p>|CPU2 FPU register read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1347|<p>MCUB VCRC register Diagnostic error</p>|CPU2 VCRC register read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1348|<p>MCUB march ram Diagnostic error</p>|CPU2 ram read/write is abnormal.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1349|<p>MCUB flash crc Diagnostic error</p>|CPU2 Flash crc value is inconsistent.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1350|<p>MCUB boot flash CRC error</p>|CPU2 boot Flash crc value is inconsistent.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the CPU2 executable.</li></ul>|
|SE1381|<p>Program sequence diagnosis error</p>|Safety controller has an abnormal sequence of safety program operations.|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1382|<p>Program sequence diagnosis error</p>|Safety controller has an abnormal sequence of safety program operations. (null_table).|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1383|<p>Program sequence diagnosis error</p>|Safety controller has an abnormal sequence of safety program operations. (number error)|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1384|<p>Program sequence diagnosis error</p>|Safety controller has an abnormal sequence of safety program operations.(local value error)|<ul><li> Reboot the controller</li><li>If the problem persists, replace the Safety controller board.</li></ul>|
|SE1500|<p>Encoder diagnostic error</p>|The encoder diagnostic results are abnormal.|<ul><li> Please reboot the controller.</li><li>Check the encoder status of the axis where the error occurred.</li><li>If the issue persists, replace the Safety Controller board. </li></ul>|
|SE1501|<p>Encoder communication error</p>|The encoder communication is abnormal.|<ul><li> Please reboot the controller.</li><li>Check the encoder cable connection.</li><li>If the issue persists, replace the Safety Controller board. </li></ul>|
|SE1502|<p>Encoder offset exceeded</p>|The deviation between the encoder value stored in the controller and the current encoder value exceeds the threshold.|<ul><li> Please reboot the controller.</li><li>Check the encoder status of the axis where the error occurred.</li><li>If the issue persists, replace the Safety Controller board. </li></ul>|
|SE1600|<p>W-phase current diagnostic error</p>|The W-phase current diagnostic result is abnormal.|<ul><li> Please reboot the controller.</li><li>If the issue persists, replace the Safety Controller board.</li><li>If the issue continues, replace the Amp board. </li></ul>|
|SE1601|<p>U-phase current diagnostic error</p>|The U-phase current diagnostic result is abnormal.|<ul><li> Please reboot the controller.</li><li>If the issue persists, replace the Safety Controller board.</li><li>If the issue continues, replace the Amp board. </li></ul>|
|SE1602|<p>UV-phase current sensor offset exceeded error</p>|The UV-phase current sensor offset exceeds the reference value.|<ul><li> Please reboot the controller.</li><li>If the issue persists, replace the Safety Controller board.</li><li>If the issue continues, replace the Amp board. </li></ul>|
|SE1603|<p>VW-phase current sensor offset exceeded error</p>|The VW-phase current sensor offset exceeds the reference value.|<ul><li> Please reboot the controller.</li><li>If the issue persists, replace the Safety Controller board.</li><li>If the issue continues, replace the Amp board. </li></ul>|
|SE1604|<p>U-phase current sensor offset exceeded error</p>|The U-phase current sensor offset exceeds the reference value.|<ul><li> Please reboot the controller.</li><li>If the issue persists, replace the Safety Controller board.</li><li>If the issue continues, replace the Amp board. </li></ul>|
|SE1605|<p>V-phase current sensor offset exceeded error</p>|The V-phase current sensor offset exceeds the reference value.|<ul><li> Please reboot the controller.</li><li>If the issue persists, replace the Safety Controller board.</li><li>If the issue continues, replace the Amp board. </li></ul>|
|SE1606|<p>W-phase current sensor offset exceeded error</p>|The W-phase current sensor offset exceeds the reference value.|<ul><li> Please reboot the controller.</li><li>If the issue persists, replace the Safety Controller board.</li><li>If the issue continues, replace the Amp board. </li></ul>|
|SE1607|<p>Current sensor disconnected</p>|Unable to read the values from the current sensor.|<ul><li> Please reboot the controller.</li><li>If the issue persists, replace the Safety Controller board.</li><li>If the issue continues, replace the Amp board. </li></ul>|
|SE1850|<p>Sequence cross check error</p>|Sequence performance results between the two CPUs are different.|<ul><li> Please reboot the controller.</li><li>If the issue persists, replace the Safety Controller board.</li><li>If the issue continues, replace the Amp board. </li></ul>|
|SE1852|<p>TCP orientation cross check error</p>|TCP orientation calculation results between the two CPUs are different.|<ul><li> Please reboot the controller.</li><li>If the issue persists, replace the Safety Controller board.</li><li>If the issue continues, replace the Amp board. </li></ul>|
|SE1853|<p>Momentum cross check error</p>|The momentum calculation results between the two CPUs are different.|<ul><li> Please reboot the controller.</li><li>If the issue persists, replace the Safety Controller board.</li><li>If the issue continues, replace the Amp board. </li></ul>|
|SE1854|<p>TCP force cross check error</p>|The TCP force calculation results between the two CPUs are different.|<ul><li> Please reboot the controller.</li><li>If the issue persists, replace the Safety Controller board.</li><li>If the issue continues, replace the Amp board. </li></ul>|
|SE1855|<p>Power cross check error</p>|The Power calculation results between the two CPUs are different.|<ul><li> Please reboot the controller.</li><li>If the issue persists, replace the Safety Controller board.</li><li>If the issue continues, replace the Amp board. </li></ul>|
|SE1856|<p>Joint position cross check error</p>|Each axis has a different command and actual axis position.|<ul><li> Please reboot the controller.</li><li>Check the version information of the system.</li></ul>|
|SE1857|TCP position cross check error|The TCP position calculated by the Main-Com and the position calculated by the safety controller are different.|<ul><li> Please reboot the controller.</li><li>Check the version information of the system.</li></ul>|

# 7.2 Warning List

| **Code** |                **Message**               |           **Cause**           | 　　　　**Solutions**                                                                                                                                     |
| :----: | :----------------------------------: | :------------------------: | ----------------------------------------------------------------------------------------------------------------------------------------------- |
|SW651|Robot safety stop violation|Robot motion has been detected in stop state.|<ul><li>Check the brake on each joint.</li></ul>|
|SW652|TCP position violation (Cell)|TCP position is out of the cell area.|<ul><li>Change the mode to manual.</li><li>Jog the robot to safety area.</li><li>Verify the job program.</li></ul>|
|SW653|Robot self collision detection|The collision detected between the robot moel and the tool model.|<ul><li>Change the mode to manual.</li><li>Jog the robot to prevent collsion.</li><li>Verify the job program.</li></ul>|
|SW654|TCP orientation violation ([deg])|TCP orientation exceeded the limits.|<ul><li>Change the mode to manual.</li><li>Jog the robot to safety area.</li><li>Verify the TCP orientation in job program.</li></ul>|
|SW655|TCP speed violation in manual mode([mm/s])|TCP speed exceeded the limits in manual mode.|<ul><li>Check the value set in the safety function menu.</li></ul>|
|SW656|Joint space violation([deg])|Joint position is out of the safe space.|<ul><li>Change the mode to manual.</li><li>Jog the robot to safety area.</li><li>Verify the job program.</li></ul>|
|SW657|Joint speed violation([deg/s])|Joint speed exceeded the limits.|<ul><li>Check the value set in the safety function menu.</li><li>Verify the joint speed in job program.</li></ul>|
|SW658|Robot power violation([N])|Robot power exceeded the limits.|<ul><li>Check the value set in the safety function menu.</li><li>Verify the joint speed and position in job program.</li></ul>|
|SW659|Robot momentum violation([kg m/s])|Robot momentum exceeded the limits.|<ul><li>Check the value set in the safety function menu.</li><li>Verify the TCP speed and position in job program.</li></ul>|
|SW660|Collision detection-safety([Axis])|If a collision occurrs, remove the cause of the collision.|<ul><li>Verify the sensitivity of collision detection.</li><li>Check the value set in the safety function menu.</li></ul>|
|SW661|TCP speed violation in reduced mode([mm/s])|TCP speed exceeded the limits in reduced mode|<ul><li>Check the value set in the safety function menu.</li><li>Verify the TCP speed in job program.</li></ul>|
|SW662|Stopping distance violation|Stopping distance exceeded the limits|<ul><li>Check the value set in the safety function menu.</li><li>Verify the robot's speed in job program.</li></ul>|
|SW663|Stopping time violation|Stopping time exceeded the limits.|<ul><li>Check the value set in the safety function menu.</li><li>Verify the robot's speed in job program.</li></ul>|
|SW664|TCP speed violation([mm/s])|TCP speed exceeded the limits.|<ul><li>Check the value set in the safety function menu.</li><li>Verify the TCP speed in job program.</li></ul>|# Attachment

# Rules on Occupational Safety and Health Standards, and Notice for Safety Inspection

The industrial robot should be installed in consideration of the inspection standards both of the Rules on Occupational Safety and Health Standards and of the Notice for Safety Inspection (if subject to inspection).

"[Rules on Occupational Safety and Health Standards](https://hrbook-hrc.web.app/#/view/rules-on-occupational-safety-and-health-standards/english/README)"
# Quality Assurance

"[Quality Assurance](https://hrbook-hrc.web.app/#/view/quality-assurance/english/README)"
