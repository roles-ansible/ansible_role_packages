[![Ansible Galaxy](https://ansible.l3d.space/svg/l3d.packages.svg)](https://galaxy.ansible.com/l3d/packages)
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
| ``l3d_pkgs__install_advanced`` | ``false`` | Install some advanced packages like tcpdump, mtr, fio and ethertools. See ``vars/main.yml`` for details |
| ``l3d_pkgs__install_python`` | ``false`` | Install some Python packages like python3-pip. See ``vars/main.yml`` for details |
| ``l3d_pkgs__install_cli`` | ``false`` | Install some CLI packages like htop, ranger and asciinema. See ``vars/main.yml`` for details |
| ``l3d_pkgs__install_extra_packages`` | | List of additional packages to install |
| ``l3d_pkgs__package_state`` | ``present`` | Package State, set to ``latest`` to upgrade packages managed by this role |
| ``l3d_pkgs__upgrade_all`` | ``false`` | Can upgrade all packages if ``l3d_pkgs__package_state`` is to ``latest`` and the value is ``true`` |
| ``l3d_pkgs__adding_ethz`` | ``true`` | Adding the swiss ETH package mirror |
| ``l3d_pkgs__ethz_contrib`` | ``true`` | contrib packages contain DFSG-compliant software |
| ``l3d_pkgs__ethz_non_free`` | ``true`` | non-free contains software that does not comply with the DFSG. |
| ``l3d_pkgs__ethz_non_free_firmware`` | ``true`` | contains non-free-firmware packages |
| ``l3d_pkgs__ethz_security`` | ``true`` | Inofficial Debian Security Mirror |
| ``l3d_pkgs__ethz_updates`` | ``true`` | Updates Mirror |
| ``l3d_pkgs__ethz__backports`` | ``true`` | Backports Mirror |
| ``submodules_versioncheck`` | ``false`` | Enable simple versioncheck to prevent running old versions of this role |

 Contributing
-------------
Please feel free to open a issue or create a pull request.
