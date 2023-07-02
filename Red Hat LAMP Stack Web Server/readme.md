# Red Hat Based LAMP Stack Web Server
Playbook creates a LAMP Stack (Apache, database server, MySQL, PHP) on Red Hat Linux based distributions.

## Resources created in Playbook

* Install Apache: Apache is the main component for hosting an http web server

* enable and start HTTPD service: enable httpd service to auto start at startup

* create httpd firewall rules: allows clients to connect to the web server

* Install MySQL: installation of sql server and hosts databases for site

* enable and start MySQL service: enable sql service to auto start on startup

* Install PHP: Installs the required files to use PHP with Apache

## Playbook Deployment
1. Run Playbook
```
sudo ansible-playbook httpd.yml -u "UserOfRemoteClient" --ask-become-pass
```
