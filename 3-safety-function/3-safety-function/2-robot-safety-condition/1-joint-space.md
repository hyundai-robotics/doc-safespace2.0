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
 
{% hint style="warning" %}
<strong>[Attention]</strong>: La fonction de sécurité effectue la surveillance sur la base de la zone définie. Cette zone doit être configurée en tenant compte de la distance d'arrêt, et une vérification doit être effectuée avant la mise en fonctionnement.
{% endhint %}
