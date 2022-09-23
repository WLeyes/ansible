# Ansible
- install ansible package

## Create an Ansible key w/out passphrase save as /home/```your_username```/.ssh/ansible
```$ ssh-keygen -t ed25519 -C "ansible" ```

## Add your ssh keys to each server
```$ ssh-copy-id -i ~/.ssh/ansible.pub YOUR_SERVER_IP ```

## Make connection to each server in inventory

```$ ansible all -m ping```

## Lists Hosts

```$ ansible all --list-hosts```

## Handy commands

```$ ansible all -m gather_facts```

```$ ansible all -m gather_facts --limit <IP Address>```
