# Azure Container Instances
Playbook creates an Azure container instance that has a connection to an Azure file share.

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
