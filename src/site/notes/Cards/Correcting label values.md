---
{"dg-publish":true,"permalink":"/cards/correcting-label-values/"}
---

up:: [[Cards/Managing issues\|Managing issues]] 
x:: 
d:: p

**Objective**: Any user can assign labels. If labels are being widely used in your Jira instance, you may need to fix incorrect values

# How to? - Bulk replace

### Search for issues with incorrect label values

Use [[Cards/Quick Search and Basic Search#Advanced search (JQL)\|JQL Search]] to search for all issues that contain incorrect values. 

For example: 

`project = PB and labels in (aples, apples)

Incorrect values can be selected from the auto-complete drop-down. Don’t include the correct value.

### Bulk replace incorrect values

Bulk change all issues by: 

1. Click Bulk change all issues > Edit issues > Change labels.
2. **Replace all with** the correct label value.
3. Next and Confirm
4. Perform quality control to make sure it all happened as expected

When you initiate the bulk change action, the incorrect label values from the search result will be replaced with the correct value.

The **Make bulk changes** global permission is required to perform bulk edits.

# Notes

## Alternative Solutions 

- *Use custom fields:* If you want to avoid [[Cards/Jira Labels\|label]] mispelling, instead of [[Cards/Correcting label values\|Correcting label values]] avoid using [[Cards/Jira Labels\|Labels]] and instead use [[Cards/Jira Components\|component]]. Another alternative is to ask the [[Cards/Jira administrator\|Jira administrator]] to configure a custom field so values can only be selected from a list. However, as with all customizations, only create custom fields when absolutely necessary. **Each new custom element in your Jira instance adds to maintenance overhead and can impact scalability**.
- *Use marketplace plugins:* Another approach to label management is to use one of the many third-party apps available in the [Jira Marketplace](https://marketplace.atlassian.com/addons/app/jira). There are several apps available that are designed to make label value entry more structured and consistent.