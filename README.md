ansible-role-neo4j
==================

![](https://github.com/kevincoakley/ansible-role-neo4j/workflows/Molecule%20Test/badge.svg)

Install Neo4j - https://www.neo4j.com . Tested with Neo4j 4.0.3 on CentOS 7, CentOS 8 and Ubuntu 18.04.

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
