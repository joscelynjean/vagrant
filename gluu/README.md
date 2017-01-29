# Gluu server installation

This Vagrantfile helps to bootstrap a Gluu server.

## Tested on

- Vagrant 1.9.1
- Virtualbox 5.0.32
- MacOS Sierra

## To run

Run this command in a terminal :

    vagrant up

Then, we need to run the following commands manually in the VM :

    vagrant ssh
    sudo /etc/init.d/gluu-server-2.4.3 login
    cd /install/community-edition-setup
    ./setup.py

The application is binded on 192.168.33.30. I usually add this entry in the hosts file.

    192.168.33.30 gluu.local

Now, you should be able to access Gluu server at https://gluu.local.
