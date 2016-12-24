## What is this?
This is the web page for laminimalteatre.cat

## Technical Info
This code contains [Trellis](https://roots.io/trellis) which is an Ansible project to manage
Wordpress projects. with dev environment throught Vagrant virtual machine.

### Secrets
This site is Open Source but we keep all password in the repo encripted with [Ansible Vault](http://docs.ansible.com/ansible/playbooks_vault.html)
If you want to work in this project you will need access to our master key. This master password is not stored in
this repo. You need to create this file `./trellis/.vault_pass` and ask for the master key to an
adminisitrator.

If you need to view some password you can do it with `view` command:
```
ansible-vault view <file>
```
File in this case could be : `./trellis/group_vars/development/vault.yml`

You can find more info here: [https://roots.io/trellis/docs/vault/](https://roots.io/trellis/docs/vault/)
