# Azure Container Instances
Playbook creates an Azure container instance running an image of httpd that has a connection to an Azure file share.

## Resources created in Playbook

----Storage Account Playbook----


* Resource Group: Container that holds related resources for an Azure solution

* Storage Account: Holds storage data

* Storage File Share: SMB based file share

* az storage account keys list: powrshell command that displays storage account keys output
* 

----Web Server Playbook----

* Azure Shell az storage directory create: creates directory in Azure File Share for container to mount

* Azure Instance Container Group: Holds a collection of containers on the same host machine

* Container: packages software into one unit that has everything the software needs to run

* Container Volume: Mounts the file share to a mount path on the container

## Playbook Deployment
Ansible is built into the Azure Cloud Shell and can be run from there.
1. Upload playbook yaml file to Azure cloud shell storage

2. install ansible galaxy collection for use of extra modules for interacting with Azure.
```
ansible-galaxy collection install azure.azcollection
```

3. Run first playbook for creating azure file share
```
ansible-playbook storageAccount.yml
```

4. Run webserver playbook
```
ansible-playbook webserver.yml
```
