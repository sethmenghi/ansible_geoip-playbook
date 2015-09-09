# geoip-playbook

Ansible playbook to install geoip python module and its dependencies. 

  $ ansible-playbook -s -kK site.yml


#### Hosts

- Edit geoip-playbook/hosts to resemble your actual host servers to appear like so:

[servers]
10.0.0.1 ansible_ssh_user=user ansible_ssh_pass=pass
127.0.0.1


(ansible_ssh_user/ansible_ssh_pass is optional)

- Then change hosts in geoip-playbook/site.yml from hosts: webservers to resemble:

hosts: servers

