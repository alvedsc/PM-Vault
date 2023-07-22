---
{"dg-publish":true,"permalink":"/cards/moving-issues/"}
---

up:: [[Cards/Managing issues\|Managing issues]] 
x:: 
d:: p

Just like in [[Cards/Correcting label values\|Correcting label values]], what you have to do is using a [[Cards/Correcting label values#How to? - Bulk replace\|Bulk replace]] 

### Use advanced issue search

From Advanced issue search ([[Cards/Quick Search and Basic Search#Advanced search (JQL)\|JQL Search]]) page, select the issues you want to move (You need the Make Bulk Changes permission)

### Choose an operation

Choose the operation "Move issues" (Requires "Move issue" permission)

### Map statuses and issue types

- Select the destination project, then begin mapping. 
- **Map issue types** in the source project to available issue types in the destination project.
- If you are moving issues with subtasks to another project, you'll also need to move the subtasks to the new project. **Subtasks must remain a subtask issue type**.
- If the source and destination projects use different workflows, **some statuses associated with the issues to be moved may not be valid in the target workflow**. In this case, you should map invalid statuses to valid statuses in your new workflow.

### Update fields for the target project

- You may need to **update required fields to match the field configuration scheme and issue types**. The same field values will be applied to all issues being moved together. You can retain original field values if you choose.
- Some fields provide a list of possible values provided for you: Component, Affects Version, Fix Version, and custom fields of type 'Version-Picker'.
- **You can't select versions that have been archived in the target project**. If you need to move issues into an archived version, you will need to first unarchive the version in the target project.

### Confirm the move

When you've specified all move parameters for all issues, there will be a confirmation screen with all your changes. The issues will be moved once you click the Confirm button. If you exit this operation before this step, your changes won't be made.

Related:
- [[Cards/Move issues (permission)\|Move issues (permission)]]