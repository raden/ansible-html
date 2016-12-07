Building a simple HTML and deploying Application using Ansible Playbooks.
------------------------------------------------------------------------

These playbooks require Ansible 2.2.0.

These playbooks are meant to be a reference and starter's guide to building
Ansible Playbooks. These playbooks were tested on redhat 7.x so we recommend
that you use RHEL or CentOS to test these modules.

This HTML can be on a single node or multiple nodes. The inventory file
'hosts' defines the nodes in which the stacks should be configured.

        [webservers]
        ip-address or hostname


Here the webserver would be configured on the local host or other node. The html can be deployed using the following
command:

        ansible-playbook -i hosts site.yml

Once done, you can check the results by browsing to http://localhost/index.html or http://ip-address/index.html
You should see a simple test.
