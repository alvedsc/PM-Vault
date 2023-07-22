---
{"dg-publish":true,"permalink":"/cards/acp-620-managing-issues/"}
---

up:: [[Cards/ACP-620 Managing Jira Projects for Cloud\|ACP-620 Managing Jira Projects for Cloud]] 
x:: 
d:: s

### Sprint management

To complete a sprint, users must be a **Jira Administrator**. Non-administrator users need **Manage Sprints** permission to manage the sprint. Since the user is a Jira administrator, Manage Sprints permission is not required.

The user requires **Edit Issues** and **Schedule Issues** because there are 2 unresolved issues that need to be moved to the backlog or to the next sprint.

**Browse Projects** is the required permission to view the issues.

**Move Issues** permission is for moving issues to another project, which is not required in managing the sprint.

**Transition Issues** grants users the ability to transition issues' status, which is not required in managing the sprint.

**Reference**:  
- [Complete a sprint](https://support.atlassian.com/jira-software-cloud/docs/complete-a-sprint/)  
- [Project permissions](https://support.atlassian.com/jira-service-management-cloud/docs/overview-of-jira-cloud-permissions/#Permissionsoverview-Projectpermissions)  
- [Permissions for company-managed projects](https://support.atlassian.com/jira-cloud-administration/docs/permissions-for-company-managed-projects/)

### Labels

All users can create labels. Therefore, the labels' value might not be consistent. Labels are also not reliable for searching because the data is not consistent. 

Labels can be used globally. It is not limited to the project level only.

Labels cannot be used in the report.

Users can use the **Bulk Change** tool to update labels' values if there are too many incorrect labels.

### Roadmap

**View Settings** is a collection of settings that allow users to adjust their personal view of the roadmap. The settings only apply to individual users. Users can change their view at any time.

**Schedule Bars** for child issues are currently available for scrum teams only.

**Epic Display Options** allow users to use the dropdown to select which epics to display. The current options are All, Incomplete, or Complete.

Users can adjust the **color** of an epic directly on the roadmap. Simply right-click the epic and choose a fresh color.

The epic bar has a default **duration** according to how users view their timeline. The default durations are weeks, months, or quarters.

Roadmaps are designed for a **single project**. It is not possible to use the roadmap if your board filters through issues from multiple projects. The roadmap helps you visualize, plan, and share work for a single project.

However, the **site administrator does not have access** to disable the roadmap.

Both team-managed and company-managed projects have a Roadmap.

Users can still **view the roadmap** without an Epic issue.

**View Read-Only Workflow** is not relevant to the Roadmap. This permission grants users access to view a read-only version of a Jira workflow.

**Reference**:   
- [Customize Your View on the Roadmap](https://support.atlassian.com/jira-software-cloud/docs/customize-your-view-on-the-roadmap/)  
- [Create Epics on the Roadmap](https://support.atlassian.com/jira-software-cloud/docs/create-epics-on-the-roadmap/)

### Component priority

Check [[Cards/Jira Components\|components]] for a specific detail of how [[Cards/default assignee\|default assignee]] is selected with [[Cards/Jira Components\|Jira Components]] 

### Epics

An epic cannot have another epic.

An epic can have issues that belong to multiple Jira projects. For example, an epic of your mobile application might include multiple Jira projects that require collaboration from multiple departments.

Both standard and sub-tasks issues type can have their own issue screen. Epic is a standard-issue type.

Users can create an Epic in the Kanban project from the **create issue screen**. Users only need to enable the **Kanban backlog** and the **Epics panel** for a particular board to manage epic in the Kanban backlog.

Users can customize Epic's colour in both Kanban and Scrum projects. The colour can be changed in the view issue screen, Roadmap, or Epics panel.

Users can move epic to other standard issue types or sub-task.

**Reference**:  
- [What is an epic](https://support.atlassian.com/jira-software-cloud/docs/what-is-an-epic/)  
- [Managing epics with the Scrum backlog](https://support.atlassian.com/jira-software-cloud/docs/manage-epics-in-a-scrum-project/)  
- [Managing epics with the Kanban backlog](https://support.atlassian.com/jira-software-cloud/docs/manage-epics-in-a-kanban-project/)

### Versions

Check more at [[Cards/Using versions and releases feature\|Using versions and releases feature]] 

The archived version will be **hidden** from the Version Report.

If you have archived issues on the board, you can view them on the board but you **cannot** release them.

Users can only **unarchive**, **merge**, **edit**, or **delete** the archived version.

Issues in the archived version are still visible on the board and JQL search. Please refer to the gif below.

**_Note:_** _By default, a Kanban board has a sub-filter_ `_fixVersion in unreleasedVersions() OR fixVersion is EMPTY_`_, which means only issues without 'fix version' or issues that have not been released yet will appear on the board. Do not confuse archiving a version with releasing a version. Kanban board will display the unreleased version on the board, and users can archive them. Those archived and unreleased versions will still appear on the board. The objective of this question is to understand the effect of archiving a version._

Users **cannot** directly move issues to the archived version. Users need to unarchive the archived version first before moving the issues. Below are steps to move issues to the archived version:

1. Unarchive the archived version.  
2. Move an issue individually or use the bulk change tool for multiple issues.  
3. Archive that version again.

### JQL 

The answer is `project = "Udemy" AND Sprint in openSprints()`. activeSprint() does not exist.

These are the only valid query for the sprint:  
- openSprints()  
- closedSprints()  
- futureSprints()

You cannot use equal sign '=' with openStrings().

You need to use 'in openSprint()'.

**Reference**: [Advanced search reference - JQL functions](https://support.atlassian.com/jira-software-cloud/docs/advanced-search-reference-jql-functions/)

