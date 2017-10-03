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
- Fill `Scheme name` and `Description Fields'
- Drag the desired issue types from from `Available Issue Types` list to `Issue Types for Current Scheme`
    - You can also create new issue types on the go, using the `Add issue type` button
- If needed, change `Default Issue type` select value to the type of your choice
- Click `Save`

Please note that this does not link project to this issue type schema. In order to perform this task, you have to click on `Associate` and select the project(s) you want to associate to the selected issue type schema.


