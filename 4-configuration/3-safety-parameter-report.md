# 4.3 安全参数报告

您可以以报告格式查看当前应用的安全参数值。
如果设置屏幕上的值尚未保存，则它们可能与报告中显示的值不同。

1. 转到您要在 `[System > 10: Safety System]` 下修改的菜单。

<p align="center">
<img src="../_assets/4/safety_report__1.png"></img>
<em><p align="center">输入安全参数设置屏幕的示例</p></em>
</p>

2. 要生成报告，请单击底部的 **\[Report]** 按钮。

<p align="center">
<img src="../_assets/4/safety_report__2.png"></img>
<em><p align="center">生成报告的示例</p></em>
</p>

3. 报告将被创建并显示在屏幕上。

<p align="center">
<img src="../_assets/4/safety__report_3.png"></img>
<em><p align="center">报告显示屏幕的示例</p></em>
</p>

4. 如果您想保存生成的报告，请单击 **\[Print]** 按钮。

<p align="center">
<img src="../_assets/4/safety__report_4.png"></img>
<em><p align="center">报告打印屏幕的示例</p></em>
</p>

5. 密码输入屏幕将出现。输入正确的密码。

<p align="center">
<img src="../_assets/4/safety_report_5.png"></img>
<em><p align="center">密码输入屏幕的示例</p></em>
</p>

6. 如果输入了正确的密码，报告将被保存，并将显示保存完成的通知窗口。

<p align="center">
<img src="../_assets/4/safety_report_6.png"></img>
<em><p align="center">报告保存完成屏幕的示例</p></em>
</p>

{% hint style="info" %}
* 安全参数由标识符 (CRC) 保护，以确保完整性。
* 该标识符是基于所有安全参数计算的，并包括与所有安全功能相关的参数。
* 当安全参数被修改时，标识符值也会变化，标识符值可以在安全参数报告的 CRC 字段中检查。
* 该标识符唯一标识所包含安全功能及其相关参数的集合。
{% endhint %}