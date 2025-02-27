[![Ansible Galaxy](https://ansible.l3d.space/svg/l3d.packages.svg)](https://galaxy.ansible.com/ui/standalone/roles/l3d/packages/)
[![BSD-3 Clause](https://ansible.l3d.space/svg/l3d.packages_license.svg)](LICENSE)
[![Maintainance](https://ansible.l3d.space/svg/l3d.packages_maintainance.svg)](https://ansible.l3d.space/#l3d.packages)

Ansible Role to install packages
---------------------

The purpose of this ansible role ist, to install some usefull packages and to give you the option to install some additional packages.
By default it will also add the [ETH Zürich Debian Packages Mirror](https://debian.ethz.ch/debian/).

 Variables
-----------

| variable | default value | useage |
| --- | --- | --- |
| ``packages__install_advanced`` | ``false`` | Install some advanced packages like tcpdump, mtr, fio and ethertools. See ``vars/main.yml`` for details |
| ``packages__install_python`` | ``false`` | Install some Python packages like python3-pip. See ``vars/main.yml`` for details |
| ``packages__install_cli`` | ``false`` | Install some CLI packages like htop, ranger and asciinema. See ``vars/main.yml`` for details |
| ``packages__install_desktop`` | ``false`` | Install some Desktop packages like thunderbird. See ``vars/main.yml`` for details |
| ``packages__install_extra_packages`` | | List of additional packages to install |
| ``packages__package_state`` | ``present`` | Package State, set to ``latest`` to upgrade packages managed by this role |
| ``packages__upgrade_all`` | ``false`` | Can upgrade all packages if ``packages__packages_state`` is to ``latest`` and the value is ``true`` |
| ``packages__adding_ethz`` | ``true`` | Adding the swiss ETH package mirror |
| ``packages__ethz_contrib`` | ``true`` | contrib packages contain DFSG-compliant software |
| ``packages__ethz_non_free`` | ``true`` | non-free contains software that does not comply with the DFSG. |
| ``packages__ethz_non_free_firmware`` | ``true`` | contains non-free-firmware packages |
| ``packages__ethz_security`` | ``true`` | Inofficial Debian Security Mirror |
| ``packages__ethz_updates`` | ``true`` | Updates Mirror |
| ``packages__ethz__backports`` | ``true`` | Backports Mirror |
| ``packages__submodules_versioncheck`` | ``false`` | Enable simple versioncheck to prevent running old versions of this role |

 Contributing
-------------
Please feel free to open a issue or create a pull request.
