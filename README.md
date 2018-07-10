# Box Descriptions
Following vagrant boxes are built from most popular based box ```ubuntu/#{code_name}64``` which usually comes with outdated version of Virtualbox Guest Addition updated to latest one as soon as new version of VirtualBox released. A vagrant plugin [vagrant-vbguest](https://github.com/dotless-de/vagrant-vbguest) is used during creating of these boxes.

## Ubuntu 18.04
[joelhandwell/ubuntu_bionic64_vbguest](https://atlas.hashicorp.com/joelhandwell/boxes/ubuntu_bionic64_vbguest/) v5.2.14
* upgraded base box version from ```ubuntu/bionic64``` from '20180522.0.0' to '20180630.0.0'
* upgraded virtualbox guest addition to version 5.2.12
* performed apt update && apt full-upgrade && apt-get autoremove
* disabled apt's periodic update

## Ubuntu 16.04
[joelhandwell/ubuntu_xenial64_vbguest](https://atlas.hashicorp.com/joelhandwell/boxes/ubuntu_xenial64_vbguest/) v5.2.14
* upgraded base box version from ```ubuntu/xenial64``` to '20180504.0.0' to '20180706.0.0'
* upgraded virtualbox guest addition to version 5.2.12
* performed apt update && apt full-upgrade && apt-get autoremove
* disabled apt's periodic update

## Ubuntu 14.04 is not supported
