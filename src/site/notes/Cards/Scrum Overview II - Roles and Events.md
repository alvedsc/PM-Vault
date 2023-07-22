---
{"dg-publish":true,"permalink":"/cards/scrum-overview-ii-roles-and-events/"}
---

up:: [[Sources/Coursework/Jira Essentials with Agile Mindset\|Jira Essentials with Agile Mindset]] 
x:: 
d:: online course

![Scrum Overview II - Roles and Events.05-05-2023.png](/img/user/Extras/Images/Scrum%20Overview%20II%20-%20Roles%20and%20Events.05-05-2023.png)

## Scrum Roles

- Three roles
	- Product Owner, Scrum Master, Development team
	- Cross-functional
	- Flexible/adaptible
	- Self-organizing (**Self-managing according to the 2020 update**)
- Stakeholders
	- Others interested in the success of the project
		- Internal - company managers, executives, other scrum teams
		- External - customers, partners, investors 

### Product owner
- Responsible for:
	- Communicating the product vision
	- Maximizing the value of each increment 
	- Responsible for the product backlog
- Interacts with, represents and is accountable to stakeholders 

### Scrum master
- Responsible for
	- Promoting and supporting scrum
	- improving the day-to-day effectiveness of the team
	- Protecting the focus of the team
	- increasing transparency of the project
- Typical task:
	- Coaching the scrum team and stakeholders on scrum
	- removing blocking issues
	- facilitating scrum events
	- configuring scrum artifacts
	- monitoring sprint progress 

#### Why are PO and SM separate?
- Two different responsibilities
	- PO - product value
	- SM - team effectiveness 
- Reasoning:
	- Divide and conquer: Lots of work on each role
	- Checks and balances: Conflicting interests
- A better alternative is to use one single Scrum Master for several teams 

### Dev team
- Cross-functional adaptive team that does the work in the project
- Responsibilities include: 
	- estimating issues
	- deciding how much work can be done in a sprint
	- deciding how to organize to do the work of the sprint
	- creating the increment of each sprint
	- ability to modify the sprint backlog during the sprint
- The scrum guide recommends three to nine members

## Scrum events

![Scrum Overview II - Roles and Events.05-05-2023-1.png](/img/user/Extras/Images/Scrum%20Overview%20II%20-%20Roles%20and%20Events.05-05-2023-1.png)

- Fixed maximum time limit, no minimum time limit (Not time-boxes)
- Meetings are primarily to plan, inspect and adapt
- Primarily about collaborating, not updating status
- Primarily spend time on things of value to all participants 

#### Sprint planning meeting
- Attendees: Entire scrum team
- Duration: Four hours for a two week sprint
- Purpose: Plan the work of the sprint
- Output: Refined sprint goal, Sprint Backlog

![Scrum Overview II - Roles and Events.05-05-2023-2.png](/img/user/Extras/Images/Scrum%20Overview%20II%20-%20Roles%20and%20Events.05-05-2023-2.png)

### Daily standup

- Attendees: Dev team + SM (Primarily)
- Duration: 15 minutes
- Purpose:
	- Inspect recent progress toward sprint goal
	- Plan the day's work
	- Identify any impediments, and plans to resolve them 
- Output: Plan for the day 

### Sprint review

- Attendees: Scrum team and stakeholders
- Duration: Typically 2 hours for a 2 week sprint 
- Purpose: Inspect the increment and collaboratively update the PB.
- Output: first-pass next sprint backlog

### Sprint Retrospective:
- Attendees: Scrum Team
- Facilitated by SM
- Duration: 90 min for a 2 week sprint
- Purpose: The team inspects itself, incluing its processes, tools and team interaction 
	- It also takes characteristics of a celebration
- Improvement issues(s) added to the next sprint's backlog 

## Summary

Any more meetings than these are discouraged as to allow the team all the time needed to complete the work 

![Scrum Overview II - Roles and Events.05-05-2023-3.png](/img/user/Extras/Images/Scrum%20Overview%20II%20-%20Roles%20and%20Events.05-05-2023-3.png)

### Kanban vs Scrum

![Scrum Overview II - Roles and Events.05-05-2023-4.png](/img/user/Extras/Images/Scrum%20Overview%20II%20-%20Roles%20and%20Events.05-05-2023-4.png)

- In Kanban, issues are in continuous flow and continous prioritization and added to the backlog
- In Scrum, each sprint has a set of issues similar to a kanban backlog, but also the timebox structure of events. Scrum is less lightweight 

## Takeaways


![Scrum Overview II - Roles and Events.05-05-2023-5.png](/img/user/Extras/Images/Scrum%20Overview%20II%20-%20Roles%20and%20Events.05-05-2023-5.png)

## Process in Jira

### Company-managed project

- Create a scrum project 
- Create issues in the PB
- Create and plan a sprint
- Execute a sprint
- Complete a sprint

- Create a scrum project 
	- Projects > Create Project button > Scrum template > Select the project type
	- Designate a project administrator (Someone who can configure the project)
		- Project Settings > People > Add people
- Create issues in the PB
	- To view backlog, click on the Backlog tab
	- Create issues there
- Create and plan a sprint
	- Click the Create Sprint button, and you'll see the Sprint Backlog show up
	- Add estimation to the issue by clicking on them and adding story points
	- You or the team members can also add subtasks here
	- Once you are finished setting up, you'll see the issues in the sprint board's sprint backlog
- Execute a sprint
	- Click on Reports tab at anytime to look at the sprints metrics, like the Burndown chart 
- Complete a sprint
	- Once all the tasks are set to DONE, you'll se a button that says: Complete Sprint


### Team managed scrum project

- Create a scrum project 
- Create issues in the PB
- Create and plan a sprint
- Execute a sprint
- Complete a sprint

- Create a scrum project 
	- Projects > Create Project button > Scrum template > Select the project type
	- If the person creating the project is not a Jira Admin, she can't create a company-managed project 
	- Name the project and select access level (open)
- Create issues in the PB
	- Enable reports (project settings > features)
	- Create issues in the backlog
- Create and plan a sprint
	- Click the Create Sprint button, and you'll see the Sprint Backlog show up
	- Add estimation to the issue by clicking on them and adding story points
	- You or the team members can also add subtasks here
	- Once you are finished setting up, click Start Sprint
- Execute a sprint
	-  Click on Reports tab at anytime to look at the sprints metrics, like the Burndown chart 
- Complete a sprint
	-  Once all the tasks are set to DONE, you'll se a button that says: Complete Sprint