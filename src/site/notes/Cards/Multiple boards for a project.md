---
{"dg-publish":true,"permalink":"/cards/multiple-boards-for-a-project/"}
---

up:: [[Cards/Board & project relationships\|Board & project relationships]] 
x:: 
d:: p

Any number of [[Cards/What is a project board\|boards]] can reference a single [[Cards/What is a Jira project\|project]]. Think of a project as a collection of tasks. A board is just one particular view of those tasks. Even though you select Kanban or Scrum when you first create a project, you’re just choosing the initial board for that project. You can use multiple boards to organize work by team or by type of work.

For example, you might want to work Stories using [[Cards/Scrum\|Scrum]] with one of your teams, and bugs and tasks with [[Cards/Kanban\|kanban]] with another team, and you only want each team to see the work relevant to them

# How to do it? 

While in the project's [[Cards/What is a project board\|board]], 
- Click on the project's dropdown (with the board name) and click on "Create board"
- Select the board you want 
- Select "Board from an existing project" 
- Fill in the details 
- Go to Board settings > scroll down to "Filter" > apply the filter you want, for example "Issue type = Story"

# Considerations

- Issues: 
	- Consider if the boards use **different issue type schemes** (and therefore have different issue types with different rules). Also, consider if the boards estimate issues differently.
- Workflow
	- **When adding a Kanban board to a Scrum project**, you may need to change the project's workflow so work can progress in the same way on both boards.  For example, if workflow conditions are tied to a particular column and that column doesn't exist in one of the boards, tasks may not be able to advance. Also, consider work in progress limits.