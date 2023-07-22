---
{"dg-publish":true,"permalink":"/cards/custom-issue-types/"}
---

up:: [[Cards/Managing issues\|Managing issues]] 
x:: 
d:: c

To understand the applicability of custom issue types check this [[Cards/case study 1 - custom issue types\|case]]

## Who can create custom issue types?

[[Cards/Jira administrator\|Jira administrators]] can create custom issue types and assign them to projects using [[Cards/Issue types\|Issue types]] schemes. However, to reduce the maintenance overhead of your Jira instance, you should always try to leverage Jira’s default issue types whenever possible.

## When should you create custom issue types?

You don't want to create issue types indiscriminately. So you need to decide when issue types are definitely needed. Such as:

-   A specific [[Cards/Jira Workflow\|workflow]] is required for a type of work
-   Different required or hidden fields.
-   Different screens when creating, editing or viewing
-   Separate reporting requirements

## What are alternatives to custom issue types?

- For example, if you need to distinguish between Internal and External Requests, this can be done with different issue types, with a Select list custom field, or even components.
- To simplify project maintenance, try to leverage Jira’s default issue types as much as possible before considering custom issue types.

# Permissions

## Jira administrator 

The [[Cards/Jira administrator\|Jira administrator]] can assign a workflow, field configuration, and screens to the new issue type in Project settings> Issue types.

They can also configure how the issue types appear when a team member creates a new issue:

-   Designate a default issue type
-   Arrange the order in which the issue types appear

## Project administrator

For all issue types, the [[Cards/Jira project administrator\|project administrator]] can configure the appearance of fields on the issue details page.

-   Order of appearance
-   Hidden when empty
-   Permanently hidden

To configure these, go to Project settings > Issue layout > Edit layout.