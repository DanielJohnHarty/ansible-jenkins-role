# ansible-jenkins-role

Ansible role used to deploy Jenkins to a server.

Configures Jenkins with administrator and tests that the web server is running on deployment.


### Example ansible deployment

```
# ./inventory/hosts

[jenkins_server]
server_01
server_02
```

```
# ./deploy_jenkins.yml

- import-playbook: ./path/to/ansible-jenkins-role/playbooks/jenkins.yml
```
