Apigee OPDK Ansible Setup Playbook
==================================

The purpose of this project is to help configure Ansible for the use of Installation of APIGEE Product. 
The Apigee OPDK roles follow conventions in the naming of files and where those files are 
located. This project sets up those locations and performs the git clone to setup your 
environment with the templates that should be customized for your use. 

Usage: Minimum Setup
====================

Set up your a workspace at ~/apigee-workspace/ if you already have git and pip installed: 

    ansible-playbook setup.yml 
    

Overview: Minimum Setup
=======================

This playbook will perform the following activities:

1. Scaffold required folders

1. Git clone of Ansible configuration file templates

1. Git clone of inventory file templates. [Updating your Inventory File]
(inventory.md)

1. Create credentials.yml template file

System Packages
===============

Required system packages can be installed with ( Optional )

    ansible-playbook install-system-packages.yml -K

Default Workspace Folders
=========================

The default workspace folders can be modified by updating workspace-folders.yml.

Default Github Repository List
==============================

The github repositories that you include can be modified by updating workspace-github-repos.yml


Scaffold required folders
=========================

This playbook will create the following folders for you: 

## ~/.ansible/configurations
Sample configuration templates for single and multi-dc planets

## ~/.ansible/inventory
Sample configuration inventory template files that model the required
 group semantics used.

## ~/.apigee
Folder to contain credentials, downloaded logs, configs and maintain the edge license.txt file.

## ~/apigee-workspace/apigee-opdk-playbook-workspace
Starter templates for playbooks. Use these playbooks as accelerators for your own.

## ~/apigee-workspace/apigee-odk-role-workspace
Workspace containing the roles used by the playbooks.