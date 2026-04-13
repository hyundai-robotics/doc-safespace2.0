# 3.3.1.5 Maintenance

The Maintenance menu allows you to set the mastering and brake test cycles. Periodic monitoring of the origin and brake status of each robot axis is essential to ensure the performance of safety functions. If the tests fail to complete within the set cycle, Safety Stop 1 is immediately activated.

To perform a brake test,

You can set the parameter values in the `[System > 10: Safety System > 1: General setup > 5: Maintenance]` menu. The Maintenance menu is configured to be accessible only to authorized users.

<p align="center">
<img src="../../../_assets/3/maintenance.png"></img>
<em><p align="center">Maintenance parameter setting screen</p></em>
</p>


|  **Parameter** |                       **Description**                       |  **Default value**  |
| :-------: | :------------------------------------------------: | :-------------: |
| <p>Mastering cycle time</p><p>[h]</p> | <p>Mastering test execution cycle</p><p>(2 ~ 720)</p> | 720 |
| <p>Break test cycle time</p><p>[h]</p>| <p>Break test execution cycle</p><p>(2 ~ 720)</p> | 720 |


{% hint style="warning" %}
<strong>[Caution]</strong>: If a crash occurs, we recommend performing a mastering test and a break test.
{% endhint %}
 