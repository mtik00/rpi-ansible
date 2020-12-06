# rpi-ansible

This is a project that I'm using to configure and maintain (at least one of) my RPis.

## Setup

You need to create a hosts file at `./instance/hosts`.  Maybe something like this:

    [rpi]
    my-pi

Install the ansible-galaxy roles with:

    ansible-galaxy install -r requirements.yml

You'll also need to create `./docker-compose-env.sh`.  This file will be copied over to the metrics server.

## Running

Pick your playbook and run it with something like:

    ansible-playbook metrics-server.yml --check
