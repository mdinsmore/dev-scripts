Scripts to manage my development process
========================================

analyse-log
-----------
Analyse a log for details of users for the site

app-status
----------
Report the git status django apps (~/repo/dev/app)

app-version
-----------
Read the version number (from the git log) of django apps and compare with 
requirements/production.txt of the current project

create-venv
-----------
Create a virtual environment and install the requirements

pip-compare
-----------
Compare the app version of the current virtual environment with the version 
specified in requirements/base.txt of the current project

pip-update-all
--------------
Update the current virtual environment to the latest versions regardless of 
the version in specified in requirements files

pull-apps
---------
Pull the latest version of django apps from the remote repository

release
-------
Release an app or project to our pypi - requires pkimber/fabric

restore-db
----------
Restore a backup script to a postgres database - requires that a variable
called CURRENT_PROJECT is set to the name of the project you wish to restore

set-branches
------------
Set the branch of all apps used by a project. Reads branch from a file called 
requirements/branch.txt in project directory.  This file should contain a line
for each app in the format: app|branch

show-commits
------------
Show the details of the commits for a repository

sshrm
-----
Remove a host from the list of known hosts

