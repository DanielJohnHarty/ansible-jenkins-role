# ansible-jenkins-role

Ansible role used to deploy Jenkins to a server running Ubuntu. No other OS are supported by this role.

Configures Jenkins with administrator and tests that the web server is running on deployment.

Requires a Java installation compatible with Jenkins (defaults to `openjdk-11-jre`).

### Example ansible deployment

```
# Generate an Ansible hosts file from `inventory/all.yml`
ansible-playbook generate-ansible-hosts-file.yml

# Run necessary preparations on server
ansible-playbook deploy-server-prerequisites.yml

# Deploy jenkins to server
ansible-playbook deploy-jenkins.yml
```
