# Set up a default permission scheme for all users in JIRA

## Introduction
JIRA, since its first startup, sets a custom permission level for every project and for every user from that moment on.

Since not all users have to create, edit or delete issues, a default permission scheme more restricted than the existent one is very useful, in order to expand it if needed, instead of limiting the group permissions on a case-by-case basis.

## How to set up JIRA

### Start from scratch
- Login to JIRA and set up the administrator user;
- Create the first project (there's no constraint on project type, it's needed in order to display the homepage)

### After first run
##### Create a user group
 - open `Settings` (gear icon) > `User management` > `Groups` (from the sidebar)
 - Fill the group name and click `Add Group` to create a new group that will have basic permissions, like `jira-core-user` (from the JIRA Core application).

##### Create a Permission Scheme

 - open `Issues` (from the top menu bar) > `Permission schemes` (at the very bottom of the sidebar)
 - create a new permission scheme clicking on `Add permission scheme` using the top-right button
 - Edit the permissions you want to grant to the group. Please note the following:
    - `Browse Projects` permission needs to be granted in order to browse issues in read-only mode
    - an issue has different parts (e.g. Comments, Workflow, Attachments..) that need to be permitted separately. 
    - A basic issue permission scheme could involve `Browse Projects`, `Create Issue` and `Edit issues`
    - Any changes can be done at any time
    - *Please note, to make a permission available to any user, either logged in or not, you have to choose the **"Anyone"** Group grant.*

##### Set permission scheme to group
The binding between permission scheme and group has already been made during permission scheme creation, on permission edit.

##### Set group default for JIRA applications
- open `Applications` (from the top menu bar) > `Application access` (second entry of the sidebar)
- Scroll to the very end of the page, until `JIRA Core` section
- Using the selection field, add the group you created before to this section, and tick the `Default` checkbox. This means the users you will create and assign to this application, will be assigned to this group by default. 
- *Please note that JIRA Software and JIRA Service Desk include JIRA Core, but **will not** assign the JIRA Core specific groups to users, if not explicitly stated.*

##### Set default application to new users
From `Application access`:
- Click on `Set defaults for new users` button
- Uncheck everything but **JIRA Core**
- close the dialog window

From now on, every user will be assigned to JIRA Core by default. You can always change the user group at any time, and select the applications directly from the User Creation wizard.

You can copy a scheme, edit an existing one (e.g. granting or restricting some permission to certain users) or delete them at any time following these instructions.


