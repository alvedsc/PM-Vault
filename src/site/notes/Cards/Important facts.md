---
{"dg-publish":true,"permalink":"/cards/important-facts/"}
---

up:: [[Cards/Managing Jira Projects\|Managing Jira Projects]] 
x:: 
d:: online course

## Difference between status and resolution

There is a difference between [[Cards/Adding statuses in Jira\|status]] and Resolution. 
- **Statuses represent the position of an issue in its workflow.** **A status can be mapped to one workflow step.** **Resolutions are the ways in which an issue can be closed**
- There's no such thing as Status = Unresolved
- There is Resoution = EMPTY 

## JQL Search inclusion of empty fields

When doing a [[Cards/JQL\|JQL]] search, Search (WHERE) statements that are stated will immediate exclude issues where the statement is non existent. For example, 

>[!Case]
>You need to write a JQL query that shows all issues, except if they are epics or have the label BETA.
>
>Identify the correct JQL query.

You might think the correct answer is `type!= Epic AND labels != BETA` but the problem is that `labels != BETA` is looking for issues with labels, immediately excluding issues without labels. The correct answer is:
- `type!= Epic AND (labels != BETA OR labels is EMPTY)`


