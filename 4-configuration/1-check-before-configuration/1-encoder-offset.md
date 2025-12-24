# 4.1.3 Encoder Inspection

Since the safety function diagnoses the robot's position and speed based on the data of the encoder mounted on each axis, the accuracy of the encoder data is important. Therefore, you should check whether the encoder values match the actual values before using the safety function.

1\. Check the home position mark of each robot axis and move the axis.


When a stop occurs due to a safety function violation, move each axis by jogging in manual mode. For detailed information on recovery methods, refer to "[**6.1 Recovery Mode**](../../6-recovery/README.md)".

2\. In the pose information window in the work area, verify that the robot's axis coordinate values are displayed as the reference posture (**0, 90, 0, 0, 0, 0** \[deg]).


* If there is no pose information window in the work area, touch the **\[+]** button at the upper right of the panel stack, then touch **\[Pose]** in the panel selection window.


3\. If the angle value error is within 0.01, proceed to the next step. If the error exceeds 0.01, perform encoder offset.

4\. Reboot the system.

{% hint style="info" %}
For more information about encoder offset, see “[**7.4.4 Encoder Offset**](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/korean-tp630/README)” in the “[**Hi6 Controller Operating Manual**](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/korean-tp630/7-system/4-robot-parameter/4-encoder-offset/README)”.
{% endhint %}
