###### Status of master branch builds: [![Build Status](https://travis-ci.com/deribinvladimir/otus201911-ansible4-db-role.svg?branch=master)](https://travis-ci.com/deribinvladimir/otus201911-ansible4-db-role)

# ansible-4 external db role

### This is just text to move ansible 'db' role to external source for my otus project https://github.com/Otus-DevOps-2019-11/deribinvladimir_infra
###### What's been done during this task:
- new repo otus201911-ansible4-db-role created and ansible db role moved into it
- service account in gcp and ssh key for tests were created, encrypted and added to .travis.yml with commands to decrypt and use it during tests
- molecule configs were modified to use gcp resources for tests
- name of role updated to external
- secure key was generated to send notifications about role repo to our personal channel in slack
- travis-ci image with build status was added to readme.md
###### Additional resources used during this homework:
- for travis setup: [how to add our repo to travis](https://docs.travis-ci.com/user/tutorial/), [about some bugs with adding repo to travis](https://github.com/travis-ci/travis-ci/issues/10137), [how to set up travis for our new external role](https://gist.github.com/Artemmkin/e1c845e96589d5d71476f57ed931f1ac), [sample of external role](https://github.com/Artemmkin/test-ansible-role-with-travis)
