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