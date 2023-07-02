# Azure web app service with SQL
Playbook creates a Windows web app with secure connection to a SQL server

## Resources created in Playbook

* App Service: Hosting Web App using App Service

* Azure SQL Database Server: Creation of Azure Databases server resource

* Azure SQL Database: Database storing website database

* Networking VNet: Connect SQL Service to App over private VNet

* Private Endpoint: Connecting SQL privatly over vnet

* App Service Vnet Integration: Connect App Service privatly to VNet

* Key Vault: Store SQL Database Admin password securly in Key Vault. secret is created at template runtime.

## Playbook Deployment

Ansible is built into the Azure Cloud Shell and can be run from the Cloud Shell

1. Set subscription to be used
```
export AZURE_SUBSCRIPTION_ID=YOURSUBSCRIPTIONID
```

2. Run playbook. Specify your subscription id at the end for setting the variable within the script.
```
ansible-playbook web_app_with_sql_ansible.yml --extra-vars AZURE_SUBSCRIPTION_ID=YOURSUBSCRIPTIONID
```
