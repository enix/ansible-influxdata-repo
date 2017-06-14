eNiXHosting.influxdata-repo for Ansible
=================

A role for deploying softare repository from [influxdata](http://www.influxdata.com). It provide Telegraf, InfluxDB, Chronograf, ... software suite.

Supports
--------

Supported targets:

- Debian 7 "wheezy"
- Debian 8 "Jessie"
- Ubuntu 16.04 "Xenial"
- RedHat EL / CentOS 6
- RedHat EL / CentOS 7

Dependencies:

- None


Usage
-----

Clone this repo into your roles directory:

    $ git clone ssh://gitlab.enix.org/ansible/ansible-influxdata-repo.git roles/influxdata-repo

Or use Ansible galaxy requirements.yml

    # eNiXHosting.influxdata-repo galaxy role
    - src: eNiXHosting.influxdata-repo
      name: influxdata-repo

And add it to your play's roles:

    - hosts: ...
      roles:
        - influxdata-repo

You can also use the role as a playbook. You will be asked which hosts to provision, and you can further configure the play by using `--extra-vars`.

    $ ansible-playbook -i inventory --extra-vars='{...}' main.yml


Still to do
-----------

- Make a var to install either local GPG key using file or by default with external url


Changelog
---------

### 1.0

Initial version.
