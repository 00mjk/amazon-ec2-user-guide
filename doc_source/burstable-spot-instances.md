# Burstable performance instances<a name="burstable-spot-instances"></a>

If you launch your Spot Instances using a [burstable performance instance type](burstable-performance-instances.md), and if you plan to use your burstable performance Spot Instances immediately and for a short duration, with no idle time for accruing CPU credits, we recommend that you launch them in [Standard mode](burstable-performance-instances-standard-mode.md) to avoid paying higher costs\. If you launch burstable performance Spot Instances in [Unlimited mode](burstable-performance-instances-unlimited-mode.md) and burst CPU immediately, you'll spend surplus credits for bursting\. If you use the instance for a short duration, the instance doesn't have time to accrue CPU credits to pay down the surplus credits, and you are charged for the surplus credits when you terminate the instance\.

Unlimited mode is suitable for burstable performance Spot Instances only if the instance runs long enough to accrue CPU credits for bursting\. Otherwise, paying for surplus credits makes burstable performance Spot Instances more expensive than using other instances\. For more information, see [When to use unlimited mode versus fixed CPU](burstable-performance-instances-unlimited-mode-concepts.md#when-to-use-unlimited-mode)\.

Launch credits are meant to provide a productive initial launch experience for T2 instances by providing sufficient compute resources to configure the instance\. Repeated launches of T2 instances to access new launch credits is not permitted\. If you require sustained CPU, you can earn credits \(by idling over some period\), use [Unlimited mode](burstable-performance-instances-unlimited-mode.md) for T2 Spot Instances, or use an instance type with dedicated CPU\.