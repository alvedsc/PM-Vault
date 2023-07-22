---
{"dg-publish":true,"permalink":"/cards/critical-path/"}
---

up:: [[Cards/Critical Path Method\|Critical Path Method]] 
x:: 
d:: c

In a [[Cards/Project Schedule Network Diagram\|Project Schedule Network Diagram]], the [[Cards/Critical path\|Critical Path]] is defined by the activities that add up to the longest completion time. For example, 

![Network Diagrams.07-07-2023.png](/img/user/Extras/Images/Network%20Diagrams.07-07-2023.png)

In this diagram, you can see three paths:
- AC -> Sums up to 7
- ADE -> Sums up to 12
- BDE -> Sums up to 14

As BDE sums up to the highest completion time, it is called the [[Cards/Critical path\|Critical path]]. 

Changes in the schedule of the activities in the [[Cards/Critical path\|Critical path]] imply changes to the whole [[Cards/Project Schedule\|Project Schedule]]. This means [[Cards/Activities (TPM)\|Activities]] in the [[Cards/Critical path\|Critical path]] have zero [[Cards/Float\|Float]]. 

> [!Note]
> If activities in other paths suffer from sufficient delay, they can become another [[Cards/Critical path\|critical path]] and even replace the current one. For example, if activity A is delayed by 2 hours, BDE and ADE would be [[Cards/Critical path\|critical paths]]. Moreover, if activity A is delayed by 3 hours, ADE would become the new [[Cards/Critical path\|critical path]].


