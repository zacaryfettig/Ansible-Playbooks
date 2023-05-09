# Windows Domain Controller Deploy Playbook
Playbook joins a computer to a Windows domain and promotes it as a domain controller.

## Playbook Deployment
1. Create an encrypted vault to store secrets in
```
sudo ansible-vault create vault_dcDeployment.yml
```


2. add in the below variables to the vault_dcDeployment.yml file

domain_ou_path: "OU=servers,DC=YOURDOMAIN,DC=COM"

domain_admin_user: DomainUsername

domain_admin_password: DomainPassword

hostname: new hostname of the server you want to add to the domain

dns_domain_name: DomainName

safe_mode_password: DomainSafeModePassword


3. Run below command in the terminal
```
ansible-playbook dcDeployment..yml --vault-password-file /etc/ansible/playbooks/vault_dcDeployment.yml
```
