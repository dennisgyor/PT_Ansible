# PT_Ansible
Upgrade ProfitTrailer bot releases via Ansible (on RP3)

## Overview
Ansible playbook to download and update the latest profittrailer releases running on Raspberry Pi 3.
There are variables that you can override on the command line. The following are
the variables and their default values:

* dl_dir: "/tmp"
* install_loc: "/home/{{ user }}/ProfitTrailer/"
* release: "https://github.com/taniman/profit-trailer/releases/download/v1.2.6.16/ProfitTrailer.zip"
* user: pi

Example:

If you want to override the user in the script, type `ansible-playbook main.yml --extra-vars "user=joe"`

You can also use this to override release information when a newer release is publicly available
on the ProfitTrailer releases [page](https://github.com/taniman/profit-trailer/releases)

.
