---
{"dg-publish":true,"permalink":"/cards/implementing-a-new-project-with-shared-configuration-using-schemes/"}
---

up:: [[Cards/Schemes\|Schemes]] 
x:: 
d:: p

Objective: To avoid having to configure new projects when the configuration is very similar to a previously created project. More info in [[Cards/Shared configuration\|Shared configuration]] 

## Implementation

Here are steps to share the configuration between an existing [[Cards/What is a Jira project\|project]] and a new project 
- To check the current project's settings:
	- Go to the project page of the project who's settings you want to use for the new project 
	- Project settings > Summary > 
		- Here you'll be able to check the current project's schemes 
- To create the new project with the shared settings 
	- Follow the process to creating a new project until selecting the "company managed project"
	- When adding in the project attributes, Enable "Share settings with an existing project" and choose the project 
	- Check the schemes using the process described above. 

>[!Note]
>Remember that if you change the settings in one project, it'll affect the other one 
