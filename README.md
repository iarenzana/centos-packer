centos-packer
=============

CentOS 6.5 / 7.0 x64 + VirtualBox / VMWare for Packer Template
Requires [Packer] (https://packer.io) and [Vagrant] (https://www.vagrantup.com).

##1) Packer Build for VirtualBox

```
cd centos6 or centos7
packer validate [ CentOS_6.5.json | CentOS_7.0.json ]
VERSION=vv20150129 packer build [ -only virtualbox-iso | -only vmware-iso ]  [ CentOS_6.5.json | CentOS_7.0.json ]
```

##2) Add Vagrant Box

```
vagrant box add iarenzana/centos6 IAR-CentOS-6.5-x86_64-vv20150129-virtualbox.box
vagrant box add iarenzana/centos7 IAR-CentOS-7.0-x86_64-vv20150129-virtualbox.box
or
vagrant box add iarenzana/centos6 IAR-CentOS-6.5-x86_64-vv20150129-vmware.box
vagrant box add iarenzana/centos7 IAR-CentOS-7.0-x86_64-vv20150129-vmware.box
```

##3) Vagrant up!

```
vagrant up
```

Enjoy!!
