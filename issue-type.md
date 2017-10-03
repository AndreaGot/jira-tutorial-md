 # Set a new issue type inside a project in JIRA
 
 ## Introduction
 It could happen that JIRA issue types are not enough for what we are trying to accomplish. It is possible to add a new one to selected projects.
 
 ## Set a new issue type
 
 ##### Create a new Issue type
- open `Settings` (gear icon) > `Issues` > `Issue types` (first entry of the sidebar)
- Click on `Add issue type` button, and fill `name` and `description` fields.
- Select which type of issue you want (`Standard` or `Sub-task`)
    - Be careful, since sub-tasks **must** be paired with a parent task

After these steps, a new issue type should appear in the list. Notice that, at the moment, it cannot be used since it is not linked to any project.

##### Link issue to project
- Click on `Issue type schemes` (second entry of the sidebar)
- You have two choices:
    - Add the new issue type to an existing issue type scheme
    - Create a new issue type scheme with this issue type (among others)

##### Add a issue type to an existing schema
- Click `Edit` next to the chosen schema
- Drag the issue type you just created from `Available Issue Types` list to `Issue Types for Current Scheme`
- Click `Save`

##### Create a new schema and add issue types
- Click on `Add Issue Type Scheme`
- 


