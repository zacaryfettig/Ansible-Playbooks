# Windows Domain Controller Deploy Playbook
Playbook creates a Windows web app with an SQL server

## Resources created in Playbook

* App Service: Hosting Web App using App Service

* Azure SQL Database Server: Creation of Azure Databases server resource

* Azure SQL Database: Database storing website database

* Networking VNet: Connect SQL Service to App over private VNet

* Private Endpoint: Connecting SQL privatly over vnet

* App Service Vnet Integration: Connect App Service privatly to VNet

* Key Vault: Store SQL Database Admin password securly in Key Vault. secret is created at template runtime.

## Playbook Deployment

1. Set subscription to be used
```
export AZURE_SUBSCRIPTION_ID=cb746d33-61f2-4005-a6e1-323245542be4
```

2. Run playbook. Specify subscription your subscription id at the end for setting the variable within the script.
```
ansible-playbook web_app_with_sql_ansible.yml --extra-vars AZURE_SUBSCRIPTION_ID=YOURSUBSCRIPTIONID
```
