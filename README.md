# Today I Learn ([@skpaik](https://skpaik.github.io "@skpaik"))

Hi! I'm Sudipta Kumar Paik. I write everthing, what I learn everyday.


## Remove Docker Containers, Images, Volumes, and Networks

Removing All Unused Objects

`sudo docker system prune`

Remove all unused volumes

`sudo docker system prune --volumes`

List of all active and inactive images
`sudo docker image ls -a`

Remove one or more images

`sudo docker image rm 75835a67d134 2a4cca5ac898`// Here '75835a67d134' & '2a4cca5ac898' is image ID

List of all active and inactive containers

`sudo docker container ls -a`

Remove one or more containers

`sudo docker container rm cc3f2ff51cab cd20b396a061` // Here 'cc3f2ff51cab' & 'cd20b396a061' is container ID


Stop and remove all containers

`sudo docker container stop $(sudo docker container ls -aq)`

`sudo docker container rm $(sudo docker container ls -aq)`

Ref: https://linuxize.com/post/how-to-remove-docker-images-containers-volumes-and-networks
>**Tech:**  `docker`, `ubuntu`

>**Date:** 2019-03-06





## Installing nano and vim in docker/Ubuntu

`apt-get update`

`apt-get install vim nano`

Ref: https://stackoverflow.com/a/37156748/705293
>**Tech:**  `vim`, `docker`, `nano`, `ubuntu`

>**Date:** 2019-03-06


## Installing MySQL in Ubuntu
Install the MySQL server by using the Ubuntu package manager:

`sudo apt-get update`

`sudo apt-get install mysql-server`

Ref: https://support.rackspace.com/how-to/installing-mysql-server-on-ubuntu/
>**Tech:**  `mysql`, `ubuntu`

>**Date:** 2019-03-04



## Uninstalling MySQL in Ubuntu

Use apt to uninstall and remove all MySQL packages:

`sudo apt-get remove --purge mysql-server mysql-client mysql-common -y`

`sudo apt-get autoremove -y`

`sudo apt-get autoclean`

Remove the MySQL folder:

`sudo rm -rf /etc/mysql`

Delete all MySQL files on your server:

`sudo find / -iname 'mysql*' -exec rm -rf {} \;`

Ref: https://help.cloud66.com/node/how-to-guides/databases/shells/uninstall-mysql.html

>**Tech:**  `'mysql'`, `ubuntu`
>**Date:** 2019-03-04


## Mongo dump and restore command
Dump or Take backup:

`mongodump -h 127.0.0.1:27017 -d dbname --out bjson_folder`

Restore to database:

`mongorestore -h 127.0.0.1:27017 -d dbname bjson_folder/dbname`


>**Here:** 

>Host = 127.0.0.1:27017(-h)

>Database name = dbname(-d)

>Dump locations BSON/JSON files = bjson_folder/(dbname auto create)(--out)

>Restore Locations of backup BSON/JSON folders = bjson_folder/dbname

>**Tech:**  `mongodb`

>**Date:** 2019-02-27


## Docker entering file system
`docker ps`

`docker exec -it name-of-container bash`
>**Tech:**  `docker`

>**Date:** 2019-02-07


## Unit Testing in ExpressJs(NodeJs)
Ref: https://codehandbook.org/unit-test-express-route
>**Tech:**  `mocha`, `nodejs`, `expressjs`

>**Date:** 2019-01-28



## Install Python & Django on Windows
Run command on Powershell

Download from https://www.python.org/downloads/

`pip install virtualenv`

`cd ~/Desktop`

`mkdir pages`

`cd pages`

`virtualenv venv`

`.\venv\Scripts\activate`

`pip install django`

`django-admin startproject app .`

`python manage.py startapp pages`

`deactivate`

Ref: https://www.codingforentrepreneurs.com/blog/install-python-django-on-windows/

>**Tech:**  `django`, `python`

>**Date:** 2019-01-23



## Activate PyCharm
Ref: https://www.codeblogbt.com/archives/282803
>**Tech:**  `pycharm`, `python`
>**Date:** 2019-01-22


## Check out a remote Git branch
`git checkout -b feature_connect_issue remotes/origin/feature_connect_issue`
Ref: https://stackoverflow.com/a/1783426/705293
>**Tech:**  `'git'`
>**Date:** 2019-01-16

## Delete Local Branch
`git branch -D branch_name`
Ref: https://stackoverflow.com/a/2003515/705293
>**Tech:**  `'git'`
>**Date:** 2019-01-16


## How To Install Linux, Apache, MySQL, PHP (LAMP) stack on Ubuntu 16.04
A "LAMP" stack is a group of open source software that is typically installed together to enable a server to host dynamic websites and web apps. This term is actually an acronym which represents the **L**inux operating system, with the **A**pache web server. The site data is stored in a **M**ySQL database, and dynamic content is processed by **P**HP.
Ref: https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04
>**Tech:**  php, mysql
>**Date:** 2019-01-10

## Faveo
Faveo is a suport ticket system.
Ref: https://github.com/ladybirdweb/faveo-helpdesk
>**Tech:**  `'php'`,`'mysql'`
>**Date:** 2019-01-10


**Table of Contents**

[TOCM]

[TOC]
