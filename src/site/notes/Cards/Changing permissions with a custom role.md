---
{"dg-publish":true,"permalink":"/cards/changing-permissions-with-a-custom-role/"}
---

up:: [[Cards/Jira Roles\|Jira Roles]]  
x:: 
d:: p

Objective: tweek specific permissions to people in your team 

# Restricting

Most issue-related permissions are granted to the default group, jira-software-users. If this default group is assigned to, for instance, the Developers project role, you might be giving broad issue permissions to users who are not part of your development team. 

Some organizations are comfortable with this situation, but others prefer exerting more control over access to the team's backlog. In this case, the project admin can just remove the default group from the project role in question, then create a custom role to grant the permission to specific users.

For example: 
- "Only the project administrator can add watchers to an issue. We'd like to give this capability to selected team members, but not make them administrators."

# Enabling

By default, the **Manage Watchers** permission is associated with the Administrators group for a project. To grant selected administrative permissions to other team members, the permissions can be associated with a custom role, and selected team members can be added to the custom role.

# Related cards:
- [[Cards/Jira administrator\|Jira administrator]] 