Scripts to manage my development process
========================================

app-status
----------
Report the git status django apps (~/repo/dev/app)

app-version
-----------
Read the version number (from the git log) of django apps and compare with 
requirements/production.txt of the current project

pull-apps
---------
Pull the latest version of django apps from the remote repository

release
-------
release an app or project to our pypi - requires pkimber/fabric

restore_database
----------------
restore a backup script to a postgres database - requires that a variable
called CURRENT_PROJECT is set to the name of the project you wish to restore

sshrm
-------
remove a host from the list of known hosts

