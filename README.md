# ansible-pi

![](https://raw.github.com/scottmotte/ansible-pi/master/ansible-pi.jpg)

Quickly setup your Raspberry Pi - particularly WIFI settings.

## Installation

1. Clone and setup the app. 

```
git clone https://github.com/scottmotte/ansible-pi.git
cd ansible-pi
cp hosts.example hosts
cp wpa_supplicant.conf.example wpa_supplicant.conf
```

2. Edit the `wpa_supplicant.conf` and `hosts` files.

3. Deploy using [ansible](http://www.ansibleworks.com). (install instructions for ansible are in [requirements](#requirements) below.

```
ansible-playbook playbook.yml -i hosts --ask-pass --sudo -c paramiko
```

## Requirements

[Ansible](http://www.ansibleworks.com/) is required. 

### Installing Ansible on Mac

```
cd /tmp
git clone git://github.com/ansible/ansible.git
cd ./ansible
git checkout v1.4.3
sudo make install
sudo easy_install jinja2 
sudo easy_install pyyaml
sudo easy_install paramiko
```

## History

This project was originally built when trying out my first Raspberry Pi. The setup process was not as easy as I wanted.
