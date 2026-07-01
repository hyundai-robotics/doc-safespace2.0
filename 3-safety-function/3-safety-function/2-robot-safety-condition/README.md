# 3.3.2 Robot Monitoring Function

Robot safety parameters consist of limit values   and stop methods for monitoring safety functions.

Each safety function can be configured with various activation conditions, stop methods upon violation, and limit values.

To configure robot safety parameters, access the menu as follows:

* `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction]`
****

The following safety features can be configured in the Robot Limits menu:

* **Joint Space**: Limits the robot's range of motion for each axis to a specific range.
* **Joint Speed**: Limits the robot's motion by preventing it from exceeding the speed limit for each axis.
* **Joint Stop**: Monitors the robot's stopped state by checking for abnormal movement for each axis after performing Stop 2.
* **TCP Speed**: Limits the robot's speed to a specified speed based on TCP standards.
* **Collision Detection**: Limits the force in the event of a collision between the robot and the worker.
* **RePlan**: Adjusts the robot's speed according to external input to perform "3.2.2 "Speed and Position Monitoring" during collaborative operation mode.
* **Power Detection**: Limits the force in the event of a collision between the robot and the worker.
* **Momentum**: Limits the energy and impact load in the event of a collision between the robot and the worker.

{% hint style="warning" %}
<strong>[Caution]</strong> : When the speed limit of any of the following safety functions is changed, it may take up to 10 ms for the new limit to become effective. In addition, for the Replan function, extra deceleration time may be required depending on the current operating conditions until the robot complies with the updated speed limit. This behavior shall be taken into consideration.
* Joint Speed Limit 
* TCP Speed Limit 
* Replan
{% endhint %}

{% hint style="warning" %}
<strong>[Attention]</strong> : Lorsque la limite de vitesse de l'une des fonctions de sécurité suivantes est modifiée, jusqu'à 10 ms peuvent être nécessaires pour que la nouvelle limite prenne effet. De plus, pour la fonction Replan, un temps de décélération supplémentaire peut être requis selon les conditions de fonctionnement actuelles, jusqu'à ce que le robot respecte la limite de vitesse mise à jour. Ce comportement doit être pris en compte.
* Limite de vitesse d'articulation (Joint Speed Limit)
* Limite de vitesse TCP (TCP Speed Limit)
* Replan
{% endhint %}

{% hint style="warning" %}
<strong>[Caution]</strong>: Operators and users must perform a risk assessment before configuring robot safety functions to ensure the safety of personnel and equipment surrounding the robot. Based on the assessment results, configure the following:

* Set a password, etc. to prevent unauthorized changes to the safety configuration.
* Configure safety-related functions and interfaces.
* Verify the accuracy of settings before operating the robot.
* Verify that all safety function configurations and settings comply with the risk assessment.
{% endhint %}

{% hint style="warning" %}
<strong>[Attention]</strong> : Les opérateurs et utilisateurs doivent effectuer une évaluation des risques avant de configurer les fonctions de sécurité du robot afin d'assurer la sécurité du personnel et des équipements situés autour du robot. Sur la base des résultats de l'évaluation, configurez les éléments suivants :

* Définissez un mot de passe, etc. pour empêcher toute modification non autorisée de la configuration de sécurité.
* Configurez les fonctions et interfaces liées à la sécurité.
* Vérifiez l'exactitude des réglages avant de faire fonctionner le robot.
* Vérifiez que toutes les configurations et tous les réglages des fonctions de sécurité sont conformes à l'évaluation des risques.
{% endhint %}