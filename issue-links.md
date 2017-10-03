# Create a new issue link in JIRA

## Introduction
Jira allows issues to be linked. It provides a couple of preset links that could be suitable in most cases, but sometimes a new one is needed. This guide will explain how to create a new link and how to use it on Issues.

## Create link between issues
##### Create link
- open `Settings` (gear icon) > `Issues` > `Issue linking` (under `Issue Features` section)
- A list with all preset links should appear. Default ones are `Blocks`, `Cloners`, `Duplicate` and `Relates`.
- Add a new link type by filling the fields underneath.
    - Pay attention to `Outward` and `Inward` description. Usually the `Outward` link is applied to the issue where the active action occurs (e.g. the issue that blocks another, or the issue that depends on another), while `Inwards` link is needed in the target issue (the blocked one, or the issue on which another depends).

##### Use link in issues
Links don't need to be added to schemes, so they are immediately effective.

In order to link two issues, do the following:
- Open the issue you want to link (either `Onward` or `Inward` one)
- From `More` menu, select `Link`
- select the `Link type`, the target `Issue`, and write a comment
- Click on `Link`

Now the two issues are linked with the selected order. You can check the link in the Issue details, under `Link` section. Please note that the target issue will have the opposite link, with regards to the one you selected.
