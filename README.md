S3-Deployment
=============

Role to get archives from S3 to deploy them to a specific folder

Requirements
------------

boto - to be able to communicate with S3

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

none

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: solutiondrive.s3-deployment }

Maintainer
----------

solutionDrive DevOps <developer@solutiondrive.de>
