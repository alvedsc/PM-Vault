---
{"dg-publish":true,"permalink":"/cards/earned-value-management/"}
---

up:: [[Cards/Control Costs\|Control Costs]]
x:: 
d:: c

- ﻿﻿Series of formulas to calculate the [[cost\|cost]] and [[schedule\|schedule]] progression of the [[Cards/Project\|project]]
	- ﻿﻿Will be done during [[Cards/Monitoring and Controlling\|monitoring and controlling]]  
		- This is not a planning tool:
		- Compares what has gotten done to the plan (plan vs. actual work)

| Term                                    | Meaning                       |
| --------------------------------------- | ----------------------------- |
| [[Cards/Budget at Completion\|BAC]]           | Budget at Completion          |
| [[Cards/Planned Value\|PV]]                   | Planned Value                 |
| [[Cards/Earned Value\|EV]]                    | Earned Value                  |
| [[Cards/Actual Cost\|AC]]                     | Actual Cost                   |
| [[Cards/Cost Variance\|CV]]                   | Cost Variance                 |
| [[Cards/Cost Performance Index\|CPI]]         | Cost Performance Index        |
| [[Cards/Schedule Variance\|SV]]               | Schedule Variance             |
| [[Cards/Schedule Performance Index\|SPI]]     | Schedule Performance Index    |
| [[Cards/Estimate at Completion\|EAC]]         | Estimate at Completion        |
| [[Cards/Estimate to Completion\|ETC]]         | Estimate to Completion        |
| [[Cards/Variance at Completion\|VAC]]         | Variance at Completion        |
| [[Cards/To-Complete Performance Index\|TCPI]] | To-Complete Performance Index |
|                                         |                               |

# You don't need to memorize anything.

It can be assumed that each planned activity delivers a fraction of the project's total value. Thus, the value of the work finished to date (Otherwise called [[Cards/Earned Value\|Earned Value]]) is the *sum of the value delivered (Value)* by all the *activities that have been completed (Schedule)*. This means [[Cards/Earned Value\|EV]] is both a measure of schedule conformance and budget conformance. 

[[Cards/Planned Value\|Planned Value]] is sort of like fiction. Once you start working, [[Cards/Planned Value\|Planned Value]] simply represents the value you should have delivered if your planned work to that date was successfully finished. This means [[Cards/Planned Value\|Planned Value]] does not represent anything related to [[Costs\|Costs]] but to work accomplishment, and thus it is a measure of conformance to the planned schedule. It simply uses a monetary value to compare it to the other value indicators, [[Cards/Earned Value\|EV]] and [[Cards/Actual Cost\|AC]]. Conversely, [[Cards/Actual Cost\|AC]] measures how much has been spent to date, regardless of the planned schedule. 

This means formulas that use [[Cards/Planned Value\|Planned Value]] only give information about the [[schedule\|schedule]], while formulas based on [[Cards/Actual Cost\|Actual Cost]] only give information about [[Costs\|Costs]].  For example, [[Cards/Cost Variance\|Cost Variance]] ($CV = EV - AC$) (Based on [[Cards/Actual Cost\|Actual Cost]]) measures the difference between the value delivered (EV) and the money spent to date (AC). If the [[Cards/Actual Cost\|Actual Cost]] exceeds the [[Cards/Earned Value\|Earned Value]], the project has spent more money than its delivered value. Conversely, [[Cards/Schedule Variance\|Schedule Variance]] ($SV = EV - PV$) measures the difference between the value delivered by the activities finished to date (EV) and the value that should have been delivered to date according to plan (PV). 

If you can grasp this, you should understand how all these formulas work without memorizing them: 
- The words *Performance Index* mean "how well it is doing." For example, a [[Cards/Cost Performance Index\|Cost Performance Index]] of 1.1 means that for every $11 of value delivered, we are spending $10. On the other hand, a [[Cards/Schedule Performance Index\|Schedule Performance Index]] of 1.1 means it has taken ten days of work to complete what we planned to complete in 11 days. 
- The word *Estimate* implies a trend. 
	- The word *at* implies the condition at a specific point. [[Cards/Estimate at Completion\|Estimate at Completion]] means the condition of the project spending if we assume the costs follow a constant trend. This implies assuming that all activities that haven't been finished will behave the same as those completed so far. Supposing that for every $11 of value delivered, we are spending $10 ([[Cards/Cost Performance Index\|CPI]] = 1.1), the forecast of the final cost of the project ([[Cards/Estimate at Completion\|EAC]]) should be lower than expected originally ([[Cards/Budget at Completion\|BAC]]). 
		- This is observable in the [[Cards/Estimate at Completion\|Estimate at Completion]] equation $EAC = BAC/CPI$. If CPI exceeds one, the [[Cards/Estimate at Completion\|Estimate at Completion]] should be lower than the [[Cards/Budget at Completion\|Budget at Completion]].  
	- The word *to* implies a transition. [[Cards/Estimate to Completion\|Estimate to Completion]] is the forecast of how much we have to pay to transition from the current state to the state of completion. In other words, [[Cards/Estimate at Completion\|EAC]] measures what is left to pay out to complete the project. It should be the difference between what has been paid out so far ([[Cards/Actual Cost\|AC]]) and what we expect to pay in total ([[Cards/Estimate at Completion\|EAC]]), and this is where the formula comes from: $ETC = EAC - AC$
- The word *Variance* implies difference. [[Cards/Variance at Completion\|Variance at Completion]] is the difference between the initially expected final cost ([[Cards/Budget at Completion\|Budget at Completion]]) and actual final cost ([[Cards/Estimate at Completion\|Estimate at Completion]]), and so the formula is $VAC = BAC - EAC$
- As the words imply, [[Cards/To-Complete Performance Index\|To-Complete Performance Index]] is "how well the project should do" from the current date on, so the [[Cards/Actual Cost\|Actual Cost]] at the end of the project equals the initial budget ([[Cards/Budget at Completion\|BAC]]). A [[Cards/To-Complete Performance Index\|TCPI]] = 1.1 means for the rest of the project expenses (BAC - AC), you can keep using $11 for every $10 value left to deliver (BAC - EV) and still finish on budget. 