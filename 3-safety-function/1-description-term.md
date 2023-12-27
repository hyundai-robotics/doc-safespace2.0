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
