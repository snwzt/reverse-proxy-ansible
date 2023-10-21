# Configuration Management with Ansible

1. Clone `https://github.com/snowset/reverse-proxy-ansible.git` to the ansible-server instance.
2. Generate SSH public key and put them in .ssh/authorized_keys file of target server.
3. Change directory to `reverse-proxy-ansible` and put IP addresses (Public or Private, depending on network) of the target server.
4. Install ansible on the target server.
5. Run `ansible-playbook -i inventory setup-playbook.yaml` to deploy the changes.
6. Run `ansible-playbook -i inventory delete-playbook.yaml` to remove the changes.