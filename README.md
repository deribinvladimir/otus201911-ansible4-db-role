###### Status of master branch builds: [![Build Status](https://travis-ci.com/Otus-DevOps-2019-11/deribinvladimir_infra.svg?branch=master)](https://travis-ci.com/Otus-DevOps-2019-11/deribinvladimir_infra)

# ansible4 db role

### ansible-3
###### What's been done during this homework:
- tasks for app and db were converted to roles using ansible-galaxy
- environments were created with group_vars for stage and prod
- playbooks were organized, ansible.cfg was updated, and deploy with new structure was checked
- community role jdauphant.nginx was added and checked to work with port 80
- ansible vault was added, credentials.yml and users.yml were created to create users and credentials.yml was encrypted by secret key
- travisci was configured to check master branch with terraform, tlint, ansible-lint and packer
###### Additional resources used during this homework:
- [jdauphant role](https://github.com/jdauphant/ansible-role-nginx)
- for some improvements of dynamic inventory (now I don't need to fix internal IP of db instance every time when env is recreated - it's assigned automatically): [gcp_compute](https://docs.ansible.com/ansible/latest/plugins/inventory/gcp_compute.html), [gather_facts](https://docs.ansible.com/ansible/latest/modules/gather_facts_module.html)
- for travis setup: [status images](https://docs.travis-ci.com/user/status-images/), [customizing the builds](https://docs.travis-ci.com/user/customizing-the-build/), [few useful samples](https://rustycrate.ru/%D0%BE%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/2017/07/30/rust-travis.html), [how to test travis config changes locally](https://medium.com/@Nklya/%D0%BB%D0%BE%D0%BA%D0%B0%D0%BB%D1%8C%D0%BD%D0%BE%D0%B5-%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D0%B2-travisci-2b5ef9adb16e)
- how to install and use tools for testing: [packer](https://www.packer.io/intro/getting-started/install.html#precompiled-binaries), [ansible-lint](https://docs.ansible.com/ansible-lint/installing/installing.html), [ansible installation with pip](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#installing-ansible-with-pip), [useful facts about pip](https://asvetlov.blogspot.com/2014/05/pip.html), [tflint](https://github.com/terraform-linters/tflint), [terraform validate](https://www.terraform.io/docs/commands/validate.html)
