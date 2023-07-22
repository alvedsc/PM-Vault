---
{"dg-publish":true,"permalink":"/cards/schemes/"}
---

up:: [[Cards/Shared configuration\|Shared configuration]] 
x:: 
d:: c

A **scheme** is a container or collection of configuration items. Schemes enable [[Cards/Jira administrator\|Jira administrators]] to create a package of configurations, then apply the package to multiple projects, eliminating the need to recreate the same configuration settings every time a new project is created. An example are [[Cards/Permission schemes\|Permission schemes]].  

![Shared configuration.14-05-2023.png](/img/user/Extras/Images/Shared%20configuration.14-05-2023.png)

Without schemes, the [[Cards/Jira administrator\|Jira administrator]] would have to configure the [[Cards/Issue types\|issue types]] for each project individually, which would be a lot of work that would need to be repeated whenever a new project was created.

## FAQ

- When would you share configurations between projects?
	- You'd do this when creating a new project that is similar to an existing project, and you believe the requirements will stay the same.
- What are the benefits of shared configurations?
	- Minimal number of unique configuration objects
	- Streamlined troubleshooting
	- Maintenance effort unaffected by growth
	- Promotes consistency
- What configurations are shared between projects?
	- Projects that share configurations share **issues types, workflows, screens, fields, permissions, notifications, and more.**
	- Lower level configurations, such as role assignments and board configurations, are project-specific and are not propagated to other shared projects.
- What happens if you change one shared project's configurations?
	- If a change is made to one of the projects' configurations, that change affects all the projects that share that configuration.

# Associated processes
- [[Cards/Implementing a new project with shared configuration using Schemes\|Implementing a new project with shared configuration using Schemes]]

