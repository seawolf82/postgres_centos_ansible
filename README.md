# postgres_centos_ansible


This script install on postgresql on Redhat based Distributions.

Tested on:

- Almalinux 8
- Almalinux 9
- RockyLinux 8
- RockyLinux 9
- Centos 7

To use postgresql_user you need to install community.postgresql from ansible-galaxy

To install it, use: ansible-galaxy collection install community.postgresql


To install postgresql on Redhat based Distributions run:

ansible-playbook -i hosts site.yaml

To uninstall postgresql on Redhat based Distributions run:

ansible-playbook -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade
package
postgres
ntp

For example, to launch only task regarding upgrade os, run:
 
ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
