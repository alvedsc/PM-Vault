---
{"dg-publish":true,"permalink":"/cards/kanban-sub-filter/"}
---

up:: [[Cards/Clearing the Done columns\|Clearing the Done columns]] 
x:: 
d:: c

A sub-filter is a feature of Kanban boards only. The sub-filter refines the results of the board filter, and goes into effect whenever the board is viewed. Explore an example query below.

**Primary filter**  
`Project = TIS ORDER BY rank ASC  
`All issues in project TIS

**Sub-filter**  
`Assignee in (currentUser())  
`Only issues assigned to the current user

# Considerations 

- When using a sub-filter, some reports may return results that differ from what's visible on the board, because **reports only look at a board’s filter query and do not factor sub-filter**.
- The default sub-filter means that issues released using the Release button no longer appear on the board, but will still show in Reports.
- To configure a Kanban board sub-filter you need project administrator privileges for the location of the board and board administrator privileges for the board itself.
- To remove a sub-filter, leave it blank.

Related:
- [[Cards/Filters\|Filters]] 