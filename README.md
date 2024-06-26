# Ansible test task

Current repo contains playbook and role collection to bootstrap new servers. It includes:

- network configuration
- cpu configuration
- storage configuration

## How to run

To run playbook you need to install dependencies:

```bash
ansible-galaxy install -r requirements
```

And run playbook itself using ansible command:

```bash
ansible-playbook -i inventories/task.yml playbooks/run.yml
```

or using taskfile if have it installed:

```bash
task run
```

## Notes

Due to it's a test repo we have `vault.key` committed.

`crypt_passphrase` - secret for drive/partition encryption. (Default: `some_secret`)

### Shell commands

There is no module for `netplan`

There is no module for `grub`

We could use ansible facts to get CPU info and detect multithreading based on `processor_threads_per_core` parameter. 
But it doesn't provide full info about CPUs, so it's better to use external tools for that. Plus external tools provide nice formatted output.
