---
{"dg-publish":true,"permalink":"/cards/gathering-business-requirements/"}
---

up:: [[Cards/Other Jira Features\|Other Jira Features]] 
x:: 
d:: p

You need to understand your team’s work style and project needs before you can create and configure a project they will want to use. This involves gathering and analyzing the team’s requirements and determining the appropriate Jira project configuration to meet those requirements. 

This task is often performed by [[Cards/Jira administrator\|Jira administrators]], but [[Cards/Jira project administrator\|project administrators]] may also be involved. **The goal is to create projects that your teams will want to use.**

## Goals of business analysis

- **Build it right the first time:** If you build it right the first time, it will reduce future overhead. Plan in advance (measure twice, cut once). Understand requirements before you start building so you don't have to backtrack or undo changes. For example, If you add in the wrong custom field types and have to migrate data later, it is a nuisance and wastes time.
- **Design it well so people want to use it** and help people get their work done more quickly and efficiently. Build a solution that doesn't become work itself, but instead gets out of the way and let's people focus on their actual job tasks. If you configure Jira well, people will want to use it, they'll have less change requests, and they'll need less training.

## Approach

To create a successful Jira configuration, it needs to relate to the business where it is being used. This can be an ongoing process, for example, when you need a new scheme or project. Or, you've had Jira for a while, but up until now, you've just used it for basic business processes and workflow and now you need something more complex. Actual implementation in Jira can be fast. Ninety-percent of the **effort is discussing and mapping out the business processes**. The main steps are:

1. Discover and understand your organization's business requirements.
2. Map those requirements to Jira configurations. 
3. Implement these configurations in Jira.

### Discover and understand your organization's business requirements.

Spend a lot of time talking with stakeholders: anyone who uses Jira, including business managers, team leads, project owners, project managers, scrum masters, iteration managers, developers, and more. 

Some questions that can help you determine the best fit:

-   Does the team plan, pull, or push work?
-   Does the team do work in a continuous flow or time-boxed periods?
-   Does the team estimate their work?
-   Does the team need a separate area to prioritize the work before it's ready for development?
-   Which agile reports does the team need?

[[Business analysis\|Business analysis]] involves drawing out the needs, and prioritization of those needs, from a group of people who have disparate interests, sometimes competing interests, and competing needs. Nailing it down the first time so you've got a really good picture that everyone can agree on. You need to understand what the long-term goals are so your Jira configuration will be good for a long time, and not just for a few weeks.

### Map those requirements to Jira configurations. 

Once you understand the business requirements, map these to Jira configurations. Plan out what changes you will make in Jira before you actually implement them. 

For example, from your stakeholder meetings you now have notes, post its and diagrams that lay out the business processes that development teams use to take their issues from creation through to completion. Now you can formalize this information into a UML or process diagram. This gives you a clear picture of what you need to implement in Jira

This includes:

-   [[Cards/Columns & Statuses\|Workflow statuses]]
-   Transitions
-   Conditions
-   Validators
-   Post functions
-   And more for each workflow. 

You also know at this point which workflow needs to apply to which development issue types: one workflow for bugs, stories, and feature requests, and another workflow for all the other issue types.

### Implement in Jira

Finally, take your business requirements that you've mapped to Jira configurations and actually implement them in Jira.  As a [[Cards/Jira project administrator\|project administrator]], you will need to work with your [[Cards/Jira administrator\|Jira administrator]] to properly configure your projects and roll them out to the team.