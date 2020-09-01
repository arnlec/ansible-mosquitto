MOSQUITTO
=========

Install and configure mosquitto service

Requirements
------------

None

Role Variables
--------------

- mosquitto_credentials
- mosquitto_ca_file
- mosquitto_cert_file
- mosquitto_key_file


Dependencies
------------

None

Example Playbook
----------------
    ---
    - hosts: localhost
      become: yes
      gather_facts: true
    
      roles:
      - role: mosquitto
        mosquitto_credentials:
          - login: user
            password: password
        mosquitto_ca_file: ca.cert
        mosquitto_cert_file: file.cert
        mosquitto_key_file: file.key

License
-------

BSD

Author Information
------------------

arnaud@lecann.com
