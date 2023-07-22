---
{"dg-publish":true,"permalink":"/cards/jira-components/"}
---

up:: [[Cards/Managing issues\|Managing issues]] 
x:: 
d:: c

**Components** group project tasks into smaller sub-sections specific to a single project. Components can represent anything: platform, location, function, content type, and more.

>[!case]
>"My team would like to organize the work in our project by certain criteria to make it easier for tracking and reporting: product feature, geographic location, and business unit."

When creating an [[Cards/Jira issues\|issue]], if you assign a component, and the component has a [[Cards/default assignee\|default assignee]] the [[Cards/Jira issues\|issue]] will be assigned the [[Cards/default assignee\|default assignee]]. However, if an [[Cards/Jira issues\|issue]] is not assigned a component, the [[Cards/Jira issues\|issue]] will be unassigned, and if you assign a component after the [[Cards/Jira issues\|issue]] has been created, the issue will remain unassigned. 

>[!info]
> Components won't allow for separate workflows. To do this, you need issue types 

## Assigning rules

Jira uses the following rules when assigning issues during issue creation.

1.  ﻿﻿﻿If the reporter selects an assignee, then the issue is assigned to that person regardless of the assignee settings at the project or component level.
2. If the reporter leaves the assignee as Automatic, then Jira checks if any components were added.
	1. If no, then Jira assigns the issue to the default assignee at the project level; which is either Unassigned or Project Lead.
	2. ﻿﻿If only 1 component was added, then Jira assigns the issue to the default assignee at the component level; which is either Project lead, Component lead, Project default, or Unassigned.
	3. If multiple components were added and one of those components has default assignee set to Component lead, then Jira assigns the issue to that person. 
	4. If multiple components were added and more than one of those has default assignee set to Component lead, then Jira assigns the issue to the component lead of the component that is first created in the system

## Associated Concepts:
- [[Cards/Jira Labels\|Jira Labels]]

## Associated processes:

- [[Cards/Creating components\|Creating components]]
- [[Cards/Using components on issues\|Using components on issues]]
- [[Cards/Viewing Components\|Viewing Components]]
- [[Using Components in reports \|Using Components in reports ]]
- [[Cards/Using Component swimlanes\|Using Component swimlanes]]


