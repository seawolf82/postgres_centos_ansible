# postgres_centos_ansible


This script install on centos7 postgresql 10


To install postgresql 10 on centos7 run:

ansible-playbook -i hosts site.yaml

To uninstall postgresql 10 on centos7 run:

ansible-playbook -i hosts deprovision.yaml
