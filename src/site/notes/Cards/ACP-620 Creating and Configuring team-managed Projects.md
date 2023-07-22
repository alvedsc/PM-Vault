---
{"dg-publish":true,"permalink":"/cards/acp-620-creating-and-configuring-team-managed-projects/"}
---

up:: [[Cards/ACP-620 Managing Jira Projects for Cloud\|ACP-620 Managing Jira Projects for Cloud]] 
x:: 
d:: s
- The Sidebar:
	- ![ACP-620 Creating and Configuring team-managed Projects.19-05-2023.png](/img/user/Extras/Images/ACP-620%20Creating%20and%20Configuring%20team-managed%20Projects.19-05-2023.png)

- **Three access levels** in team-managed Jira projects: 
	- **Open** - Anyone with access to the site can search, view, create, or edit this project's issues.
	- **Limited** - Anyone with access to the site can search, view, and comment on this project's issues. Only people added to the project can create and edit its issues.
	- **Private** - Only admins and people added to the project can search, view, create, or edit its issues.

**Reference**: [Manage how people access your team-managed project.](https://support.atlassian.com/jira-software-cloud/docs/manage-how-people-access-your-team-managed-project/#Managehowpeopleaccessyournext-genproject-deleteRole)


- Permissions
	- A team-managed project is suitable for teams that want to control their own working processes and practices in a self-contained space. You can mix and match agile features to support your team as you grow in size and complexity.
	- Team-managed projects configurations do not impact other projects.
	- Users can create a new project role in a team-managed project.
	- All licensed users can create a team-managed project, even non-admins. If you are a Jira admin and want to restrict this, you need to update the 'Create team-managed projects' global permission.
	- Users cannot allow anonymous access to a team-managed project. If users want to allow anonymous access, Jira administrators need to create a company-managed project for them.
	- Only **company-managed** projects can run parallel sprints.
- Reference: [What are team-managed and company-managed projects.](https://support.atlassian.com/jira-software-cloud/docs/what-are-team-managed-and-company-managed-projects/)


- **Team-managed** software projects come with **three roles** by default:  
	- **Administrator** - Admins can do most things, such as: update settings, add other admins to the project, manage features, customize issue types, and add rules on the board. Admins need product access to Jira Software to get the full benefit of this role.
	- **Member** - Members are a part of the team. They can create issues, edit them, comment on them, move them into different statuses, and generally collaborate on the project's work. Members need product access to Jira Software to get the full benefit of this role.
	- **Viewer** - Viewers can search through and view issues in the project, but not much else. You can give any registered user on your Jira site this role without extra product access.

- [[Cards/Jira Roadmaps\|Jira Roadmaps]] : 
	- Both team-managed and company-managed projects have a Roadmap.