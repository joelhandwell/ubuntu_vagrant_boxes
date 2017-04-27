# Box Descriptions
Following vagrant boxes are built from most popular based box ```ubuntu/#{code_name}64``` which usually comes with outdated version of Virtualbox Guest Addition updated to latest one as soon as new version of VirtualBox released. A vagrant plugin [vagrant-vbguest](https://github.com/dotless-de/vagrant-vbguest) is used during creating of these boxes.

[The issue with official ubuntu/xenial64 image not having sudo user vagrant](https://bugs.launchpad.net/cloud-images/+bug/1569237) is also addressed for xenial.

## Ubuntu 16.04
[joelhandwell/ubuntu_xenial64_vbguest](https://atlas.hashicorp.com/joelhandwell/boxes/ubuntu_xenial64_vbguest/) v5.1.20
* upgraded base box version from ```ubuntu/xenial64``` '20170418.0.0' to '20170425.0.0'
* virtualbox guest addition is version 5.1.20
* performed apt update && apt full-upgrade && apt-get autoremove
* created user vagrant with sudo and vagrant default ssh key access
* disabled apt's periodic update
* ensured ```/sbin/mount.vboxsf``` correctly linked

## Ubuntu 14.04
[joelhandwell/ubuntu_trusty64_vbguest](https://atlas.hashicorp.com/joelhandwell/boxes/ubuntu_trusty64_vbguest) v5.1.20
* upgraded base box version from ```ubuntu/trusty64``` '20170412.0.0' to '20170422.0.0'
* upgraded virtualbox guest addition to version 5.1.20
* performed apt update && apt full-upgrade && apt-get autoremove
* ensured ```/sbin/mount.vboxsf``` correctly linked

## Ubuntu 12.04
[joelhandwell/ubuntu_precise64_vbguest](https://atlas.hashicorp.com/joelhandwell/boxes/ubuntu_precise64_vbguest) v5.1.20
* upgraded base box version from ```ubuntu/precise64``` '20170404.0.0' to '20170417.0.1'
* upgraded virtualbox guest addition to version 5.1.20
* performed apt-get update && apt-get dist-upgrade && apt-get autoremove
* ensured ```/sbin/mount.vboxsf``` correctly linked

## Ubuntu 16.04 desktop
[joelhandwell/ubuntu_xenial64_desktop_vbguest](https://atlas.hashicorp.com/joelhandwell/boxes/ubuntu_xenial64_desktop_vbguest) v5.1.20
* base box is ```box-cutter/ubuntu1604-desktop``` 'v2.0.26'
* upgraded virtualbox guest addition to version 5.1.20
* performed sudo apt update -y && sudo DEBIAN_FRONTEND=noninteractive apt-get -y -o Dpkg::Options::="--force-confdef" -o Dpkg::Options::="--force-confold" dist-upgrade && sudo apt-get autoremove -y
* ensured ```/sbin/mount.vboxsf``` correctly linked
