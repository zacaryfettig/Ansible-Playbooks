# Rucks ICX Network Automation using Ansible
Playbooks used to make ICX configuration changes using Ansible. Ansible uses ssh to login to the network switches and uses the comscope.icx collection modules to run commands on the switches.


## Playbook Deployment


1. install ansible galaxy collection for use of extra modules for interacting with Azure.
```
ansible-galaxy collection install commscope.icx 
```

2. install ansible-pylibssh for added capability to ssh to network devices
```
Sudo pip install ansible-pylibssh 
```

3. Run a playbook to change configuration of Ruckus ICX network switch.
```
ansible-playbook rebootICX.yml
```
