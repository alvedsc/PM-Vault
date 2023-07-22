---
{"dg-publish":true,"permalink":"/cards/parallel-sprints/"}
---

up:: [[Cards/Other Jira Features\|Other Jira Features]] 
x:: 
d:: c

Check this case:

>[!Case]
>"We have multiple teams working from the same backlog, and they need to run their sprints simultaneously. Can we run additional sprints at the same time?"

If the [[Cards/Jira administrator\|Jira administrator]] enables **parallel sprints** for the entire Jira instance, projects can have multiple active sprints. However, **all teams will need to use the same [[Cards/Agile Estimation\|Estimation]] metric since they are working from a common backlog.**

Keep in mind that, when running the Velocity Chart report against the project, the report will not segment velocity by individual team

What if you want to show several sprints on the same board, separated by categories? 
Check [[Cards/Showing parallel sprints on a board\|Showing parallel sprints on a board]]

When running [[Cards/Parallel sprints\|Parallel sprints]], only one sprint can be completed at a time. To complete a sprint:

- Select the **Sprint** drop-down.
- Select a single sprint.
- Then select **Complete sprint.**

[[Cards/Parallel sprints\|Parallel sprints]] are not enabled by default. You need to ask the [[Cards/Jira administrator\|Jira administrator]] to enable them at 
- Settings > Products > Jira software configuration > Enable

Now, if you are using the [[Cards/Scrum\|Scrum]] template, you'll be able to impement the parallel sprints. 
- In the **Backlog tab**, that's where you create the sprints and assign the issues. 
	- RIght above the backlog and below any already existing sprints, you'll see a button that says "Create sprint". Click and and add the issues to the new sprint. 
	- Then click on "Start Sprint" > Add the sprint attributes and click Start
- Now, go above the board, you'll see a sprint that says "All sprints". Click there and select the sprint you who's issues you want to display 

# Related cards:

- [[Cards/Shared configuration\|Shared configuration]] 
- [[Cards/Board Configuration\|Board Configuration]] 

