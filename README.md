Role Name
=========

Upgrade all packages and reboot if required.

Requirements
------------

[Community General Collection](https://galaxy.ansible.com/community/general)

Role Variables
--------------

None.

Dependencies
------------

None.

Example Playbook
----------------

    ---
    - name: upgrade all packages and reboot if required
      hosts: "{{ target }}"
      gather_facts: true

      roles:
        - unix_upgrade

License
-------

BSD

Author Information
------------------

Jørn Ivar Holland
