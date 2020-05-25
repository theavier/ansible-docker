# ansible-docker


Running this Playbook will install docker and docker-compose locally using ansible 

1. Obtain the playbook
git clone https://github.com/theavier/ansible-docker.git

2. Run the Playbook
ansible-playbook -i hosts  deploy.yml --ask-become-pass
