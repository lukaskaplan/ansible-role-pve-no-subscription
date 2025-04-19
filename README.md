pve_no_subscription
=========

This ansible role should be used if you are using Proxmox VE without paid support. There is annoying popup window with the warning about missing subscription.

This role turns off the subscription warning and sets "no-sbscription" apt repositories.

Requirements
------------

Proxmox VE running on the target host.

Role Variables
--------------

`pve_no_subscription_proxmoxlib_path` - you don't need to change it. It is paath to the edited file.

Dependencies
------------

No dependencies.

Example Playbook
----------------

```yaml
- name: Example playbook
  hosts: proxmox_servers

  tasks:
    - name: Turn off subscription warning
      include_role: 
        name: pve_no_subscription
```

License
-------

MIT
