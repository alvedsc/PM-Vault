---
{"dg-publish":true,"permalink":"/cards/acp-620-boards-and-projects/"}
---

up:: [[Cards/ACP-620 Managing Jira Projects for Cloud\|ACP-620 Managing Jira Projects for Cloud]] 
x:: 
d:: s

- If users are creating a new board (Kanban or Scrum) with multiple Jira projects, and each project has a unique workflow, all statuses will be mapped to 3 default columns: **To Do, In Progress, and Done**.
	- On the **Kanban board**, the issues will appear on the board as soon as users created the board.
	- On the **Scrum board**, the issues will not appear on the board. After creating a new Scrum board, you do not have an active sprint. Only issues in the active sprint will appear on the Scrum board.

- Board is just a way to view your issues. Users can create multiple Scrum or Kanban boards on any Scrum or Kanban project.
	- When creating the Kanban board on a Scrum project, these configurations might need to be updated:
		- Issue Type schemes  
		- [[Cards/Agile Estimation\|Estimation]] methods  
		- Work-in-progress limits  
		- Custom workflows
	- For example, the 'Backlog' and 'Selected For Development' statuses from the Scrum board will be grouped under the 'To Do' column in the Kanban Board. There will be a lot of issues in the 'To Do' column.
	- **Reference**:  
		- [Create a board](https://support.atlassian.com/jira-software-cloud/docs/create-a-board/)  
		- [Configure a company managed board](https://support.atlassian.com/jira-software-cloud/docs/configure-a-company-managed-board/)