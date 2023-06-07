# Windows Domain Controller Deploy Playbook
Playbook creates a Windows web app with an SQL server

## Playbook Deployment

1. Set subscription to be used
```
export AZURE_SUBSCRIPTION_ID=cb746d33-61f2-4005-a6e1-323245542be4
```

2. Run playbook. Specify subscription your subscription id at the end.
```
ansible-playbook web_app_with_sql_ansible.yml --extra-vars AZURE_SUBSCRIPTION_ID=YOURSUBSCRIPTIONID
```
