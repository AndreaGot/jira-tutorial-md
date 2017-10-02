## Set up a default permission scheme for all users in JIRA

### Introduction
JIRA, since its first startup, sets a custom permission level for every project and for every user from that moment on.

Since not all users have to create, edit or delete issues, a default permission scheme more restricted than the existent one is very useful, in order to expand it if needed, instead of limiting the group permissions on a case-by-case basis.

### How to set up JIRA

If you start from scratch, the following two steps can be skipped. 

- Login to JIRA and set up the administrator user;
- Create the first project (there's no constraint on project type, it's needed in order to display the homepage)

 From now on, this guide applies to every user:
 
 - open `Settings` (gear icon) > `User management` > `Groups` (from the sidebar)
 - Fill the group name and click `Add Group` to create a new group that will have basic permissions, like `jira-core-user` (from the JIRA Core application).
 - open `Issues` (from the top menu bar) > `Permission schemes` (at the very bottom of the sidebar)
 - create a new permission scheme clicking on `Add permission scheme` using the top-right button
 - Edit the permissions you want to grant to the group. Please note the following:
    - `Browse Projects` permission needs to be granted in order to browse issues in read-only mode
    - an issue has different parts (e.g. Comments, Workflow, Attachments..) that need to be permitted separately. 
    - A basic issue permission scheme could involve `Browse Projects`, `Create Issue` and `Edit issues`
    - Any changes can be done at any time

