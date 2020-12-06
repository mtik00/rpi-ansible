# rpi-ansible

This is a project that I'm using to configure and maintain (at least one of) my RPis.


## Setup

You need to create a hosts file at `./instance/hosts`.  Maybe something like this:

    [rpi]
    my-pi

## Running

Pick your playbook and run it with something like:

    ansible-playbook metrics-server.yml --check
