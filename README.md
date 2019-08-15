ansible-role-neo4j
==================

[![Build Status](https://travis-ci.org/kevincoakley/ansible-role-neo4j.svg?branch=master)](https://travis-ci.org/kevincoakley/ansible-role-neo4j)

Install Neo4j - https://www.neo4j.com . Tested with Neo4j 3.5.8 on CentOS 7 and Ubuntu 18.04.

Requirements
------------

None

Role Variables
--------------

See defaults/main.yml

Dependencies
------------

None

Example Playbook
----------------

    - name: Neo4j role for Ubuntu systems
      hosts: neo4j
      become: yes
      become_method: sudo
    
      vars:
        neo4j_allow_any_connection: true
    
      roles:
        - ansible-role-neo4j
    
      tags:
        - neo4j

License
-------

BSD

Author Information
------------------

Kevin Coakley (https://github.com/kevincoakley)
