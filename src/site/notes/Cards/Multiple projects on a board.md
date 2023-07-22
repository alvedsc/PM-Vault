---
{"dg-publish":true,"permalink":"/cards/multiple-projects-on-a-board/"}
---

up:: [[Cards/Boards & Projects\|Boards & Projects]] 
x:: 
d:: p


# Creating a New Board

One way to associate multiple projects with a board is to create a new board, selecting the option to create the board from an existing project.

Then, in the Project field, specify multiple projects.

Even though the board will query multiple projects, it still has a home project as indicated by the Location field. This simply means the board will be grouped together with other boards from the indicated project, but this does not determine what the board can display.

In this example, even though the board’s Location is Project B, the board is not required to display issues from Project B.

![Multiple projects on a board.12-05-2023.png](/img/user/Extras/Images/Multiple%20projects%20on%20a%20board.12-05-2023.png)

- A [[Cards/What is a project board\|board]] is just a way to view your issues. Users can create multiple Scrum or Kanban boards on any [[Cards/Scrum\|Scrum]] or [[Cards/Kanban\|kanban]] project.
	- When creating the Kanban board on a Scrum project, these configurations might need to be updated:
		- Issue Type schemes  
		- [[Cards/Agile Estimation\|Estimation]] methods  
		- Work in progress limits  
		- [[Cards/custom workflow\|custom workflow]]
	- For example, the 'Backlog' and 'Selected For Development' statuses from the Scrum board will be grouped under the 'To Do' column in the Kanban Board. There will be a lot of issues in the 'To Do' column. 

- Regarding projects with different [[Cards/Columns & Statuses\|Columns & Statuses]], and [[Cards/Jira Workflow\|workflows]], whenever you add [[Cards/Multiple projects on a board\|Multiple projects on a board]], and each project has a unique workflow, all statuses will be mapped to 3 default columns: **To Do, In Progress, and Done**.
	- On the **Kanban board**, the issues will appear on the board as soon as users created the board.
	- On the **Scrum board**, the issues will not appear on the board. After creating a new Scrum board, you do not have an active sprint. Only issues in the active sprint will appear on the Scrum board.
	- **Issues won't be hidden from the board**. They'll just default to the **To Do, In Progress, and Done** config. 

![Multiple projects on a board.19-05-2023.png](/img/user/Extras/Images/Multiple%20projects%20on%20a%20board.19-05-2023.png)


# Modifying a Board

You can create a ONE BOARD MANY PROJECTS relationship, by following the instructions at [[Cards/Modify the board filter\|Modify the board filter]]. One thing you want to do if you make a relationship like this is to configure the swimlanes (as it appears in [[Cards/Enrich Issues#^f237ff\|here]]). 
- More information on how to do this in [[Cards/Board Configuration\|Board Configuration]]: 
	- For this case, the [Base swimlanes on] dropdown should show "Projects"


# Organizing projects

To keep the board better organized, you can configure swimlanes by project, so each project’s issues appear in their own swimlane, making it easy to distinguish issues from the different projects.


