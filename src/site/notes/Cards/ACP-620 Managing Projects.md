---
{"dg-publish":true,"permalink":"/cards/acp-620-managing-projects/"}
---

up:: [[Cards/ACP-620 Managing Jira Projects for Cloud\|ACP-620 Managing Jira Projects for Cloud]] 
x:: 
d:: s

# Roles

**Site administrators:**  
- Usually someone that has the authority to manage the team's finances.  
- Manage new users.  
- Manage billing and subscriptions.  
- Manage site settings.

**Jira administrators:**  
- Usually someone that has good technical knowledge in Jira.  
- Manage Jira plugins.  
- Manage Jira global configurations (Global permissions, global settings, etc).  
- Manage Jira schemes (Workflow, permissions, screens, notifications, etc).

**Project administrators:**  
- Usually someone that is managing a specific Jira project.  
- Manage project configurations (Roles, project details, etc).

**Jira Software users:**  
- Users that are working on issues in the Jira Software project.  
- Users' permissions are being managed by other administrators.

# [[Cards/Shared configuration\|Shared configuration]] 

More info at [[Cards/Shared configuration\|Shared configuration]] 

Jira will **not** copy the below configurations if users created a project using the **shared configuration option**. These configurations are associated with a single Jira project and cannot be shared across other projects:

- Components  
- Version  
- Project role members  
- Project avatar  
- Project description  
- Project URL (From Details page)

# Project fields

In the Jira project 'Details' page, users can only change:

- Name  
- Key  
- URL  
- Project category  
- Avatar  
- Description  
- Project lead  
- Default assignee

Users cannot change their Jira project type. To change the project type, users need to create a new project and use the 'Bulk Change' tools to move all issues into the new project. 

**Reference:**  
- [Convert a project to a different template or type](https://support.atlassian.com/jira-cloud-administration/docs/convert-a-project-to-a-different-template-or-type/)  
- [Edit a project's details](https://support.atlassian.com/jira-cloud-administration/docs/edit-a-projects-details/#Editingaproject-sdetails)

# Archiving projects 

Users can **archive** inactive projects along with their issues, components, attachments, and versions. This won’t affect associated schemes, workflows, issue types, or any content that is shared with other projects. When a project is archived, its issues won’t appear in basic or advanced search results. Users can still access these issues through direct links, but you won’t be able to edit them.

A **hidden** project will still be visible to people with admin permissions; regular users won't be able to search, view or modify any of the project's issues.

Users can get rid of projects that they don't need by moving them to **trash**. The projects along with its issues, components, attachments, and versions will be available in the trash for 60 days, after which they will be permanently deleted. Associated schemes, workflows, issues types, or any content that could be shared with other projects won't be affected. Issues from projects in trash won't appear in issue search results.

To permanently **delete** a project, users must first move the project to trash. Once they permanently delete a project from the trash, they won't be able to recover it. If they think that they might need the project later, it is recommended to either archive projects or hide projects instead.

**Reference:**  
- [Hide a project](https://support.atlassian.com/jira-cloud-administration/docs/hide-a-project/).  
- [Archive a project](https://confluence.atlassian.com/adminjiracloud/archive-a-project-1013843066.html).  
- [Trash for Jira Cloud projects](https://support.atlassian.com/jira-cloud-administration/docs/trash-for-jira-cloud-projects/).  
- [Delete a project](https://support.atlassian.com/jira-cloud-administration/docs/delete-a-project/).