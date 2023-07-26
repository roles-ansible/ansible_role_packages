
Ansible Role to install packages
---------------------

```
WARNING: REWRITE
```

A base ansible role that should run on common Linux systems.

This role adds more package sources to Debian. And installs some useful tools. This role adds more package sources to Debian. And installs some useful tools. The complete list of tools to install can be found in the [vars/main.yml](https://github.com/roles-ansible/ansible_role_base/blob/master/vars/main.yml).

Optionally you can also set vim as the default editor and update all packages to ``latest``.


### variables:

For a complete overview of all variables have a deeper look into the ``vars`` nd the ``defaults`` Folder!.

```yml
---
# install these additional packages
base__extra_packages: []
# - foo
# - bar

# should we add additional package source?
base__add_ethz: true

# add nonfree/firmware packages?
base__pkg_non_free_firmware: true
base__pkg_contrib: true

# add security repo
base__pkg_security: true

# add Debian Volatile
base__pkg_updates: true

# optionaly print some OS vars
base__print_os_vars: false

# choose latest or present for package state
# set this to latest for updating all packages!
base__package_state: 'present'

# should we update all packages?
base__upgrade_packages_to_latest_version: false

# install keychain (ssh agent)
base__install_keychain: true

# install vim (comand line editor)
base__install_vim: true

# perform a simple versions check (true is recomended)
submodules_versioncheck: false
```
