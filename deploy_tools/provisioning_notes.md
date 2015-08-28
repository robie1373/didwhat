Provisioning a new site
=======================

## required packages

* nginx
* python3
* git
* pip
* virtualenv

e.g. on Ubuntu:

    sudo apt-get install nginx git python3 python3-pip
    sudo pip install virtualenv

## nginx virtual host config

* see nginx.template.conf
* replace SITENAME with, e.g. staging.my-domain.com

## Upstart job

* see gunicorn-upstart.template.conf
* replace SITENAME with, e.g. staging.my-domain.com

## Folder structure:
Assume we have a user account at /home/username

/home/username
|
----sites
    |
    --- database
    |
    ---source
    |
    ---static
    |
    ---virtualenv