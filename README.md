Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

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

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
