---
{"dg-publish":true,"permalink":"/cards/jira-subtasks/"}
---

up:: [[Cards/Default issue types\|Default issue types]] 
x:: 
d:: c

Subtasks represent smaller, more granular work items. They create a child issue, that is related to their parent task. Subtasks are created within the context of a parent task. A single task can have multiple subtasks. The ability to have subtasks in Jira can be disabled by the Jira administrator. 



- Sub-tasks can have different workflows than their parents 
- Sub-tasks won't appear in reports. Only stadard issues will
- Sub-tasks can appear nested in the [[Cards/Board Configuration\|board]] if you select the "Base swimlanes on Stories" option 
- If there is a sub-task holding up the resolution of an issue, **users can convert the sub-task to a standard issue type**, allowing it to be worked on independently. 
- If an issue is really just a sub-task of a bigger issue, **users can also convert an standard issue type to a sub-task**.
- Using the **Bulk Change** tool, users can convert and move multiple sub-tasks to standard issue types to the same project/other projects.
- Sub-tasks cannot have another sub-task.
- Sub-tasks are **enabled by default**. Users can disable sub-tasks if there are no sub-tasks created in any of the users' Jira applications.
- Users can add '**Sub-Task**' translations for the installed languages. Any translations users define in the Sub-Task Translations page will override any translations that may exist for the issue constants in their languages resource bundle. To revert to the resource bundles values, users need to set the name/description pair to blank.

Examples:

-   Update video codec
-   Modify data input function
-   Schedule design review

Note that when you create a subtask, the following values are inherited from the parent task:

-   project
-   issue security level
-   sprint value (if any)