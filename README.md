# My dev station

**Not tested on clean install, do not use yet**

This ansible playbook installs my dev station on Ubuntu.

Packages installed:
 * atom.io
 * git
 * gitg
 * zsh
 * docker
 * samba
 * pinta
 * f.lux

Set unity conf : Cycle through multiple sizes
Set autostart : atom.io, terminal and f.lux

Prerequisites:
```
sudo apt-add-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install software-properties-common ansible
```

How to get:
```
wget https://github.com/niweb21/MyDevStation/archive/master.zip
unzip master.zip
```

How to run:
```
cd MyDevStation-master
ansible-playbook -i local main.yml --ask-sudo-pass
```

**TODO:**
- [ ] Complete readme
- [ ] set conf atom.io
- [ ] set conf git / git id
- [ ] template zsh conf
- [ ] environement user variable
- [ ] test on clean ubuntu install
- [ ] docker purge lxc-docker
- [ ] tag role
- [ ] improved quality
- [ ] elegant way to become root user
- [ ] ...

Thank to:
- Michael Aquilina for his [apm library](https://github.com/MichaelAquilina/ubuntu-ansible/blob/master/library/apm)
- lbischof for his [gsetting library](https://github.com/lbischof/ansible-gsetting)
