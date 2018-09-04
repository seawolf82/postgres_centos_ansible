# postgres_centos_ansible


This script install on centos7 postgresql 10


To install postgresql 10 on centos7 run:

ansible-playbook -i hosts site.yaml

To uninstall postgresql 10 on centos7 run:

ansible-playbook -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade
package
postgres
ntp

For example, to launch only task regarding upgrade os, run:
 
ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
