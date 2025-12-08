# 3.3.1.5 Maintenance

The Maintenance menu allows you to set the mastering and brake test cycles. Periodic monitoring of the origin and brake status of each robot axis is essential to ensure the performance of safety functions. If the tests fail to complete within the set cycle, Safety Stop 1 is immediately activated.

To perform a brake test,

You can set the parameter values ​​in the **\[System > 8: Safety System > 1: Basic Settings > 5: Maintenance]** menu.

<p align="center">
<img src="../../../_assets/3/maint_param.png"></img>
<em><p align="center">유지 보수 설정 화면</p></em>
</p>


|  **Parameter** |                       **Description**                       |  **Default value**  |
| :-------: | :------------------------------------------------: | :-------------: |
| <p>Mastering execution cycle</p><p>[h]</p> | <p>Mastering test execution cycle</p><p>(2 ~ 720)</p> | 720 |
| <p>Break test execution cycle</p><p>[h]</p>| <p>Break test execution cycle</p><p>(2 ~ 720)</p> | 720 |


{% hint style="warning" %}
**\[Caution]**: If a crash occurs, we recommend performing a mastering test and a break test.
{% endhint %}
 