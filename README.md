# Ansible

## Installation

### MacOs

Using `homebrew`

```
brew install ansible
```

### Linux

Using `pip` or `pipx`

https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html

For specific distro

https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html

## Prepare Baremetal

Current usage will require ssh keys to be added to the target machine so that password don't have to be entered for ansible to run.

Copy ssh keys to machine
```
ssh-copy-id -i <path-to-ssh-key> <user>@<ip>
```
The above command also automatically adds the host key fingerprint. This will allow ansible to run more smoothly without additional user input.