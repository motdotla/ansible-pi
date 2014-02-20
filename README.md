# ansible-pi

Quickly setup your Raspberry Pi - particularly WIFI settings.

## Installation

```
cp hosts.example hosts
cp wpa_supplicant.conf.example wpa_supplicant.conf
```

Edit the wpa_supplicant.conf and hosts files.

Deploy using [ansible](http://www.ansibleworks.com). (install instructions for ansible are in [requirements](#requirements) below.

```
ansible-playbook playbook.yml -i hosts --ask-pass --sudo -c paramiko
```
