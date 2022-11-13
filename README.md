# mongo4_centos

This script install mongodb CE version 4.4 on Red Hat Based Distributions

Tested on:

- Almalinux 8
- Almalinux 9
- RockyLinux 8
- RockyLinux 9
- Centos 7

Tested on:

- 2.9 Ansible version


To install mongo4 on Red Hat Based Distributions run:

ansible-playbook -i hosts site.yaml

To uninstall mongo4 on Red Hat Based Distributions run

ansible-playbook -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade
package
ntp
mongodb


For example, to launch only task regarding upgrade os, run:
 
ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
