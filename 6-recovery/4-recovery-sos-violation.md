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
