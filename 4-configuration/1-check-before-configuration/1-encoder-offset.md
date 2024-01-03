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
