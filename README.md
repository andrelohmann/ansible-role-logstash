logstash
========

Simple role to install logstash your machine.

!!! This role doesn't take security into account. Shipping of data should be secured by iptables. !!!

!!! This role builds the counterpart to https://galaxy.ansible.com/andrelohmann/elasticstack !!!

Role Variables
--------------

    elasticsearch_listen_ip: "localhost" # ip address to which logstash should connect to
    elasticsearch_release: 7.16.2
    elasticsearch_logstash_syslog_config: False # install a sample syslog config
    elasticsearch_syslog_index: syslog-direct

Example Playbook
----------------

    - hosts: logstash
      roles:
         - { role: andrelohmann.logstash }

License
-------

MIT

Author Information
------------------

https://github.com/andrelohmann
