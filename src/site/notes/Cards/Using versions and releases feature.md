---
{"dg-publish":true,"permalink":"/cards/using-versions-and-releases-feature/"}
---

up:: [[Cards/Clearing the Done columns\|Clearing the Done columns]] 
x:: 
d:: p

Objective: Controling which issues show in the board, organizing work by grouping issues by version released, [[Cards/Clearing the Done columns\|Clearing the Done columns]] in project boards, and giving you milestones to aim for in your work. 

Issues can be grouped in Jira, for both [[Cards/Kanban\|kanban]] and [[Cards/Scrum\|scrum]], by associating them with succesive versions. This is an optional feature managed by [[Cards/Jira project administrator\|project administrator]]s and used in Jira Software or Jira Core. Versions are defined in the project and are for that project only; they are not global. When you release a version, it removes the associated [[Cards/Jira issues\|issues]] from the board. 

>[!case]
>"I'm using Jira to manage the development of a product. I've defined different versions to help me track which issues relate to different phases of my product."

**Versions with a release date will automatically be highlighted as "overdue" if the version is unreleased when that date passes.**

# How to do it? 

- Go to the project page
- Find the "Releases" tab
- Click on "Create version"
	- Add details in the pop-up
- When you are creating a new [[Cards/Jira issues\|issue]] you can assign the version in the "Fix versions" dropdown
- In each issue, you can see the "version" field in the attributes. You can change the version directly on the issues there 

## Creating and assigning versions 

Issues can be assigned to versions from the backlog or from an issue’s Fix versions field. You will require the Edit Issues permission.  
  
As a Project administrator, you also have the option to create new versions.

The Releases page displays the status of all versions, including previously released versions. New versions can be created from this page, as well.

Clicking a version will display additional details and provide the option to release the version.

## Releasing versions 

After clicking a version on the Releases page, the Release hub is displayed, providing a dashboard with real-time visibility into the status and progress of an upcoming release. Also, the Release Hub, when integrated with other Atlassian development tools, automatically identifies issues that are marked complete but still have open pull requests or require reviews, as well as any other un-reviewed code or open builds. 

By ensuring that a completed issue is truly complete, Release Hub mitigates risks, replaces time-consuming status update meetings, and provides for a more confident and stress-free release process for the entire team.

**Clicking the Release button will release the version.**

Versions can be released from:
-   Releases board menu
-   Releases page

If there are unresolved issues in the version you are releasing, you can choose to move them to the next version in the pop-up

>[!info]
>**Released issues are removed from board except if the issues are currently in an active sprint.**

# Pros & Cons

## Pros

-   Useful for software projects with designated updates
-   Bundles released issues together
-   Creates audit trail through the release history

## Cons

-   Unnecessary overhead for non-software projects that don’t need to track versions
-   Generates metadata that may not be relevant to project
-   Can generate unnecessary notifications
- Jira does not retain versions when moving an issue to a different project. Versions are project specific 