Provisioning a new site
============================

## Required packages:

* nginx
* python 3.6+
* virtualenv + pip
* Git

## Nginx Virtual Host config

* see nginx.template.conf
* replace SITENAME with, e.g. staging.my-domain.com

## Sytemd service

* see gunicorn-systemd.template.service
* replace SITENAME with, e.g. staging.my-domain.com
* replace wsgi application

## Folder structure:
Assume we have a user account at /home/username

/home/username
-- sites
---- SITENAME
------ database
------ source
------ static
------ virtualenv
