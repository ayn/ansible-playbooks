# Ansible Ubuntu 12.04 LTS stacks

ref: [LAMP server-playbooks](https://github.com/fourkitchens/server-playbooks) and [5 minutes bootstrap](https://github.com/phred/5minbootstrap/)

`carmudgeons.yml` provisions a LAMP digitalocean droplet


`wordpress.yml` provisions a LAMP digitalocean droplet with Wordpress multisite install

## Setup Instructions

This assumes you have Ansible installed, look at [getting started](http://ansible.cc/docs/gettingstarted.html) to get setup

    # cd ~/work/ansible && source hacking/env-setup
    # cd - && ansible-playbook wordpress.yml -u root

After initial provisioning, root ssh access will be disabled, you will need to run `-K` to get prompted for sudo password:

    # ansible-playbook wordpress.yml -K

