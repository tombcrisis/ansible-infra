# Ansiblizing Proxmox

In the interest of repeatability, I upgraded a lot of my one-off home infrastructure by putting the provisioning behind [ansible](https://www.ansible.com) playbooks.

This wouldn't be possible without the excellent [ansible proxmox module](https://docs.ansible.com/ansible/latest/modules/proxmox_module.html).

This work establishes a few ansible roles
* [localized](https://github.com/tombcrisis/ansible-infra/tree/master/roles/localized) - Force a host to use a specific local file encoding
* [ntp](https://github.com/tombcrisis/ansible-infra/tree/master/roles/ntp) - Synchronize a host with NTP servers
* [proxmox_node](https://github.com/tombcrisis/ansible-infra/tree/master/roles/proxmox_node) - Provision a host to be a proxmox node
* [proxmox_lxc](https://github.com/tombcrisis/ansible-infra/tree/master/roles/proxmox_lxc) - Create and provision a proxmox container on a proxmode node

There are also a few samples for how to apply these roles.
