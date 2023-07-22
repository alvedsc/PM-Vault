---
{"dg-publish":true,"permalink":"/cards/creating-an-automation-rule/"}
---

up:: [[Cards/Jira Automation\|Jira Automation]] 
x:: 
d:: p

Project settings > Automation > Rules > Create Rule


1. Select a trigger
	1. The trigger is an event or situation that initiates the automation rule. In this example, the trigger is **Issue created**.
2. Select conditions
	1. Conditions narrow the scope of the automation rule so it only executes actions under specific circumstances.  This example automation rule uses an **Issue fields condition** to examine the Issue type field.
3. Select actions
	1. Actions accomplish something based on your trigger and conditions. In this example, the **Create subtasks action** automatically creates one or more subtasks related to the blog post.
4. Name the rule and turn it on
	1. You can give the rule a descriptive name, like **Create blog post subtasks**, and click Turn it on.
5. Test the rule
	1. You should always test your rule by creating situations in which it should trigger and should not trigger. Here, we'd create a new issue with an Issue type of task to see if the rule **automatically creates subtasks**.
6. Check the audit log
	1. Each automation rule has an **audit log** that displays when the rule was modified or run, and if the run was a success. Click on Show more to see details.

# Notes

- Automations belong to [[Cards/What is a Jira project\|projects]] but [[Cards/Jira administrator\|Jira administrator]]s can set global rules in the automation rules jira administration page
- `If: <issue type> exists ` only considers whether it exists in relation to the issue that the automation is looking at. 
	- For example, an issue has a Parent Epic. `If: Epic exists` will select this issue for automation because the Epic exists as a parent. 