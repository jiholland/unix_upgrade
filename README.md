Role Name
=========

Upgrade all packages and reboot if required.

Requirements
------------

[Community General Collection](https://galaxy.ansible.com/community.general)

Role Variables
--------------

None.

Dependencies
------------

None.

Example Playbook
----------------

    ---
    # ansible-playbook playbook_unix_upgrade.yml -e "target=localhost" --ask-become-pass
    - name: upgrade all packages and reboot if required
      hosts: "{{ target }}"
      gather_facts: true
      gather_subset: min

      roles:
        - unix_upgrade

License
-------

BSD

Author Information
------------------

Jørn Ivar Holland
