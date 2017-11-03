# Box Descriptions
Following vagrant boxes are built from most popular based box ```ubuntu/#{code_name}64``` which usually comes with outdated version of Virtualbox Guest Addition updated to latest one as soon as new version of VirtualBox released. A vagrant plugin [vagrant-vbguest](https://github.com/dotless-de/vagrant-vbguest) is used during creating of these boxes.

[The issue with official ubuntu/xenial64 image not having sudo user vagrant](https://bugs.launchpad.net/cloud-images/+bug/1569237) is also addressed for xenial.

## Ubuntu 16.04
[joelhandwell/ubuntu_xenial64_vbguest](https://atlas.hashicorp.com/joelhandwell/boxes/ubuntu_xenial64_vbguest/) v5.2.0
* upgraded base box version from ```ubuntu/xenial64``` 'v20171011.0.0' to 'v20171028.0.0'
* upgraded virtualbox guest addition to version 5.2.0
* performed apt update && apt full-upgrade && apt-get autoremove
* created user vagrant with sudo and vagrant default ssh key access
* disabled apt's periodic update

## Do not support Ubuntu 14.04, 12.04 and Ubuntu 16.04 desktop
