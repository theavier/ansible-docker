# ansible-docker
Settings

    create_containers: number of containers to create.
    default_container_name: default name for new containers.
    default_container_image: default image for new containers.
    default_container_command: default command to run on new containers.

Running this Playbook

Quick Steps:
1. Obtain the playbook

git clone https://github.com/do-community/ansible-playbooks.git
cd ansible-playbooks/docker_ubuntu1804

2. Customize Options

nano vars/default.yml

#vars/default.yml
---
create_containers: 4
default_container_name: docker
default_container_image: ubuntu
default_container_command: sleep 1d

3. Run the Playbook

ansible-playbook -l [target] -i [inventory file] -u [remote user] playbook.yml
