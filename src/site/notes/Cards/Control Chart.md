---
{"dg-publish":true,"permalink":"/cards/control-chart/"}
---

up:: [[Cards/Jira Reports\|Jira Reports]]
x:: 
d:: c

The control chart measures a team’s **cycle time, which is the total time issues spend on work until they are done**. Measuring cycle time is an efficient and flexible way to improve a team's processes because the results of changes are discernable almost immediately, allowing them to make any further adjustments right away. The end goal is to have a consistent and short cycle time, regardless of the type of work. While cycle time is a primary metric for Kanban teams, Scrum teams can benefit from optimized cycle time as well.

![Control Chart.13-05-2023.png](/img/user/Extras/Images/Control%20Chart.13-05-2023.png)

- Y-axis: days between "In progress" and "done"
- X-axis: date when issues transition to "done"
- Orange line: average cycle time for all issues
- Blue line: rolling average cycle time for all issues at a given time 
- Green dots: Individual issues (open circle) or multiple issues (solid circle). Dots above the lines indicate cycle times longer than average, while dots below the lines indicate faster throughput by the team.
	- You can click on the green dots to get information on the specific issue or the cluster

# Notes

Teams with shorter cycle times are likely to have higher throughput, and teams with consistent cycle times across many issues are more predictable in delivering work. Some tips:

-   Don't be concerned with every outlier; look for trends.
-   The goal is consistent cycle times for work items with similar point values.
-   Filter the control chart for each story point value to check for consistency.
-   Look for causes during retrospectives and improve future estimations.

# Related issues

- [[Cards/Cycle time\|Cycle time]]
