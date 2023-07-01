# Azure Container Instances
Playbook creates an Azure container instance that has a connection to an Azure file share.

## Playbook Deployment
Ansible is built into the Azure Cloud Shell and can be run from there.
1. Upload playbook yaml file to Azure cloud shell storage

2. Open cloud shell in Azure portal and change directory to yaml file location
```
cd cloudrive
```

3. Run below command in the terminal
```
ansible-playbook web_app_with_sql_ansible.yml
```
