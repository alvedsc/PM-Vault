---
{"dg-publish":true,"permalink":"/cards/configuring-team-managed-projects/"}
---

up:: [[Cards/Creating & Configuring Team-managed Projects\|Creating & Configuring Team-managed Projects]] 
x:: 
d:: p

The foundation of every [[Cards/Jira issues\|Jira issues]] is its key, summary, and status. But, some tasks require more information to help the team take on that work. How would you meet this requirement?

# Configuring issue types

- What can you configure for different issue types?
	- [[Cards/Jira project administrator\|project administrator]]s can customize each issue type to show different fields. You can add, reorder or remove fields and also create custom fields.
- What are the default fields?
	- By default, Jira adds a few fields to your issue types that we think help provide context to your project's work: Summary, Description, Status, Assignee, Reporter, and Labels. Jira also comes with a few commonly-used fields you might consider adding, for example, Priority and Due Date.
- Where do fields added to issue types appear?
	- When you add a field you select what part of the issue you want it to appear in: Description, Context or Hidden.

>[!info]
> **Don’t add too many fields as this can confuse users and they will often leave half of them empty, which creates bad data.**

To check which issue types a project has, go to
- Project > Project settings > Issue types 

To add a new issue  
- Click on "Add issue type"
- Add details

To edit issue types, 
- Click on the issue type you wanna edit
- Check the list of issue types to the right

# Configuring boards & projects

## Board configurations
There are many board configurations available, but these are common ones:

-   Customize your team-managed project board by dragging columns to be in any order you want.
-   Set column limits to highlight a column if its issue limit is exceeded.
-   Click + to create new columns, but don’t add too many columns as the board will become difficult to use.

## Project configurations
Team-managed projects are very flexible. You can start with the features of a Kanban project and, as your needs change, you can add features to make it a scrum project, like by turning on Sprints and Estimation. You can change these features at any time, so it doesn't matter what template you initially choose when creating a team-managed project.

You can also add apps. Atlassian Marketplace apps add new functionality to your team-managed projects. Use them to integrate third-party tools and add-ons into your project. When your Jira administrator integrates third-party apps to your Jira site, project administrators might have the option to display or hide the app's functionality in their team-managed projects and adjust their settings. Go to Project settings > Apps.

>[!info]
>**Team-managed projects don't have schemes, so any changes made in a team-managed project apply only to that project.**
>
**If, for example, you add a new issue type to a project, when you go to the Issue Types Jira administration page, you won't see the issue type there. That page only shows company-managed project issue types.**
