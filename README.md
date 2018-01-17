# Box Descriptions
Following vagrant boxes are built from most popular based box ```ubuntu/#{code_name}64``` which usually comes with outdated version of Virtualbox Guest Addition updated to latest one as soon as new version of VirtualBox released. A vagrant plugin [vagrant-vbguest](https://github.com/dotless-de/vagrant-vbguest) is used during creating of these boxes.

## Ubuntu 16.04
[joelhandwell/ubuntu_xenial64_vbguest](https://atlas.hashicorp.com/joelhandwell/boxes/ubuntu_xenial64_vbguest/) v5.2.6
* upgraded base box version from ```ubuntu/xenial64``` '20171212.0.0' to '20180112.0.0'
* upgraded virtualbox guest addition to version 5.2.6
* performed apt update && apt full-upgrade && apt-get autoremove
* user vagrant was found in base box, so no need to create this newly any more! 
* disabled apt's periodic update

## Do not support Ubuntu 14.04, 12.04 and Ubuntu 16.04 desktop
