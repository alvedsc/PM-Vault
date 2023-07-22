---
{"dg-publish":true,"permalink":"/cards/kanban/"}
---

up:: [[Sources/Coursework/Jira Essentials with Agile Mindset\|Jira Essentials with Agile Mindset]] 
x:: 
d:: online course

![Kanban Method.04-05-2023.png](/img/user/Extras/Images/Kanban%20Method.04-05-2023.png)


## Kanban Method overview

- ![Kanban Method.04-05-2023-1.png](/img/user/Extras/Images/Kanban%20Method.04-05-2023-1.png)
- Kanban method is an agile method to manage a contonuous queue of work items 
- Commonly used ideas: 
	- Visualize work
	- Remove process bottlenecks to improve "flow" of value
	- Limit work in progress
	- Pull work rather than push (Where it makes sense)
	- Continuously prioritize work items

### Why Kanban
- Lightweight and efficient
- Evolutionary approach of transforming to Agile (from traditional)
- Works well if the workflow is service oriented
	- Operations
	- Support
	- Maintenance development
	- New hire funnel
- Supports multi-team and multi-project workflows 


## Improving flow

![Kanban Method.04-05-2023-2.png](/img/user/Extras/Images/Kanban%20Method.04-05-2023-2.png)

- How to improve flow
	- Specify the minimum or maximum number of issues allowed in certain project board columns (WIP: Work in Progress)
	- Why
		- Better flow: finishing work items that are started
		- Limits waste: finishing items instead of multitask
		- Promotes teamwork: When there are bottlenecks, the team works together to eliminate them

### WIP Limits 
#### Column under minimum limit
- It is the minimum number of items in a column
- When the number of items is less than the min, the column turns yellow
- It is an effective way to ensure there's always available work for the team to pull from

#### Column under maximum limit
- Column turns red when the number of items in the column exceeds the max
- It is an effective way to prevent the team from multitasking and not finishing what they start 

#### How to set the WIP Limits
- You could start with no limits ad see how the team progresses
	- If there are no problems, then no limits need to be set
	- Adding WIP limits  to discourage multitasking and improve flow
	- Set WIP limits on steps the team tends to neglect 
- ==How? 
	- Company-wide: Go to Board Settings > Columns > Add the numbers to each column you need
	- Team-wide: Each column has a "Column limit" option in its "..." menu

### Agile Reports
- Visualize the work of the team
- Promotes transparency
- Aid in troubleshooting and continuous improvement
- Aid in planning and estimating 

#### Cumulative flow diagram
Shows the number of issues per status over time 

![Kanban Method.04-05-2023-3.png](/img/user/Extras/Images/Kanban%20Method.04-05-2023-3.png)

You can see many things:
- Bottlenecks
- Flow improvement
- How well the team keeps up with the backlog

You can't see individual issue problems, but you have other reports for this purpose

How to show the CFD?
- Company wide: Left panel > Reports > Cumulative Flow Diagram
- Team Wide: Reports need to be added to the interface first 
	- Left panel > Project settings > Features > enable reports 
	- Back to project > Select CFD 

## Pull vs Push

![Kanban Method.04-05-2023-4.png](/img/user/Extras/Images/Kanban%20Method.04-05-2023-4.png)
Check how in this example, each team member etiher pushes or pulls from a queue in a kitchen

Now check the same example in a Jira project 
![Kanban Method.04-05-2023-5.png](/img/user/Extras/Images/Kanban%20Method.04-05-2023-5.png)


Now what happens when you add a Review step? 
![Kanban Method.04-05-2023-6.png](/img/user/Extras/Images/Kanban%20Method.04-05-2023-6.png)

It is not clear whether the developer pushes the item into review, or the reviewer pulls it... 
Solution? Add a Development Done Queue! 

![Kanban Method.04-05-2023-7.png](/img/user/Extras/Images/Kanban%20Method.04-05-2023-7.png)

### Why pull? 
- Empowers the team: Team members select their work, instead of assigning it to them 
	- *This is basic also un Scrum. Remember the team decides the HOW*
- Mantains a sustainable pace, since the team members decide when they are ready for what 

## Separate backlog (To plan work)

- The backlog contains items that are not ready to be worked on... 
- Why?
	- May need more information
	- May never be prioritized for work 
- Team members can't work on Backlog items
	- So Jira can separate the backlog from the project board
- How?
	- Company wide: Board Settings > Columns 
		- Drag the Backlog status to the left
		- ![Kanban Method.05-05-2023.png](/img/user/Extras/Images/Kanban%20Method.05-05-2023.png)
	- Team Wide: Project Settings > Features > Backlog
		- Once it is there, you have to drag issues to the board in the backlog page
	- Once you select this option, you can access the backlong in a different page (Backlog on the left panel)
	- ![Kanban Method.04-05-2023-8.png](/img/user/Extras/Images/Kanban%20Method.04-05-2023-8.png)


## Takeaways

![Kanban Method.04-05-2023-9.png](/img/user/Extras/Images/Kanban%20Method.04-05-2023-9.png)


