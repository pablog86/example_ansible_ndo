# NDO static binding using Ansible
Example of static binding using Ansible on Cisco NDO.

Create a csv file using the example sheet in the same folder of the playbook and run it with:

- For only configuration of the template:

> ANSIBLE_HOST_KEY_CHECKING=False ANSIBLE_PERSISTENT_COMMAND_TIMEOUT=60 ansible-playbook -i host2.yml NDO-static-binding2.yml -t only-conf -v

- For configuration and deploy of the template:

> ANSIBLE_HOST_KEY_CHECKING=False ANSIBLE_PERSISTENT_COMMAND_TIMEOUT=60 ansible-playbook -i host2.yml NDO-static-binding2.yml -t deploy -v

PD: Edit the host2.yml with the IP, User and pass of your NDO deployment.
