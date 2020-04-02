# proxmox_ansible

promox_ansible is a collection of Ansible roles and playbook that automate the installation of Proxmox.

Current roles are:

- ansible-os-hardening - hardening by [dev-sec](https://github.com/dev-sec/ansible-os-hardening)
- host_prep
- proxmox


## Supported Linux Distributions

 - **Debian** Buster

## Setting hostname, domain name and LAN range

You can define these here: 

host_prep/vars/main.yml


## Running it

To run the playbook, populate an inventory file:

```ShellSession
[proxmox]
1.2.3.4

[proxmox:vars]
ansible_python_interpreter=/usr/bin/python2
```

Finally, run ansible:

```ShellSession
ansible-playbook proxmox.yml -i inventory
```

## Contributing

Contributions are welcome. Feel free to open a pull request with changes.
