---
{"dg-publish":true,"permalink":"/cards/use-cases/"}
---

up:: [[Cards/Managing Roles and Permissions\|Managing Roles and Permissions]] 
x:: 
d:: s

> [!Case]
> "Certain team members need to be able to delete issues, which normally only administrators can do. But, we don't want to give full administrator permissions to these team members; they only need to be able to delete issues."
 
By default, only administrators have the ability to delete issues. How would you meet this requirement?

Solution: 
- First, as a [[Cards/Jira administrator\|Jira administrator]] 
	- Creates a [[Cards/Changing permissions with a custom role\|custom project role]] (e.g., Issue Managers)
	- Creates a new [[Cards/Permission schemes\|Permission schemes]] (e.g., Development Permission Scheme)
	- Assigns the Delete issues permission to the custom role
	- Associates the Development Permission Scheme with the project
- Then, as [[Cards/Jira project administrator\|Jira project administrator]] 
	- Adds selected project users to the Issue Managers custom role

> [!info]
> **If this requirement wasn’t limited to selected projects, but applied to all Jira projects, creating a new scheme wouldn’t be necessary. The Jira administrator could simply modify Jira’s Default software permission scheme that is applied to all Jira projects by default.**

---

> [!Case]
> "For certain projects, we need specific users to be able to start and stop sprints. By default, any Jira Software user can start/stop sprints. How can we allow only selected users to manage sprints?"

Solution: 
- First, as a [[Cards/Jira administrator\|Jira administrator]] 
	- Creates a custom project role (e.g., Scrum Master)
	- Creates a new permission scheme (e.g., Development Permission Scheme)
	- Updates the Manage sprints permission so it only applies to the Scrum Master custom role 
	- Associates the Development Permission Scheme scheme with the project
- Then, as [[Cards/Jira project administrator\|Jira project administrator]] 
	- Adds selected project users to the Scrum Master custom role


