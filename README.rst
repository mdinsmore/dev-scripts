Scripts to manage my development process
========================================

Some scripts to aid the development process mostly for development
using python and django on Linux.  They assume you have a directory
structure as follows::

  ~
  |
  +-- bin  # program and scripts directory 
  |
  +-- dev
       |
       +-- app   # directory for django apps
       |
       +-- module  # directory for documentation, deployment info etc
       |
       +-- project  # django projects directory

Installation
============

To use simply clone this repository and then change to the dev-scripts
directory type::

  ./create-bin

This will create a directory called ~/bin/ if it does not already exist.
You should add this directory to your PATH.

Scripts provided
================

analyse-log
-----------
Analyse a log for details of users for the site

app-status
----------
Report the git status django apps (~/dev/app)
(-v or --verbose displays the remote origin)

app-venvs
---------
Recreate the virtual environments for all apps

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

project-venvs
---------
Recreate the virtual environments for all projects

pull-apps
---------
Pull the latest version of django apps from the remote repository

recreate-venv
---------
Recreate the virtual environment for the current directory

release
-------
Release an app or project to our pypi - requires pkimber/fabric

requirements
------------
check a virtual environment pip requirements file against a reference file

restore-db
----------
Restore a backup script to a postgres database - requires that a variable
called CURRENT_PROJECT is set to the name of the project you wish to restore

restore-files
-------------
Restore a files backup to the media (and if it exists media-private)
directory of the specified project directory

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

watch-folder
------------

watch a folder an perform an action if there's a change.  This is a python
script required python3

watch-docs
----------

Uses watch-folder and to monitor a sphinx documentation directory and 
build the html if there's a change.
