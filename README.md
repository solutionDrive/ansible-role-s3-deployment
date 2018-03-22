S3-Deployment
=============

Role to get archives from S3 to deploy them to a specific folder

Requirements
------------

boto - to be able to communicate with S3

Role Variables
--------------

    project_name: 'project'
The project_name will be used for the full installation_path

    installation_path: '/var/www/'
Installation path which will hold the project name directories

    download_destination_path: '/tmp/'
Destination path to store the archive temporary

    download_destination_file: "{{ download_destination_path }}release.tar.gz"
Filename to use for storing the archive

    owner: 'www-data'
Owner which will be set to the files/folders in the installation_path/project_name folder

    group: 'www-data'
Group which will be set to the files/folders in the installation_path/project_name folder

    s3_bucket: ''
Bucket which should be used

    s3_object: ''
Object which should be downloaded from the bucket
    
    aws_region: 'eu-central-1'
Region in which the bucket is available

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
