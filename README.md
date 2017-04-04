# Box Descriptions
Following vagrant boxes are built from most popular based box ```ubuntu/#{code_name}64``` with latest Virtualbox Guest Addition. [The issue with official ubuntu/xenial64 image not having sudo user vagrant](https://bugs.launchpad.net/cloud-images/+bug/1569237) is addressed.

## Ubuntu 16.04
[joelhandwell/ubuntu_xenial64_vbguest](https://atlas.hashicorp.com/joelhandwell/boxes/ubuntu_xenial64_vbguest/) v5.1.1820170331
* upgraded base box version from '20170330.1.0' to '20170331.0.0'
* virtualbox guest addition is version 5.1.18
* performed apt update && apt full-upgrade && apt-get autoremove
* created user vagrant with sudo and vagrant default ssh key access
* disabled apt's periodic update

## Ubuntu 14.04
[joelhandwell/ubuntu_trusty64_vbguest](https://atlas.hashicorp.com/joelhandwell/boxes/ubuntu_trusty64_vbguest) v5.1.18
* upgraded base box version from 'v20170302.0.0' to 'v20170313.0.0'
* upgraded virtualbox guest addition to version 5.1.18
* performed apt update && apt full-upgrade && apt-get autoremove

## Ubuntu 12.04
[joelhandwell/ubuntu_precise64_vbguest](https://atlas.hashicorp.com/joelhandwell/boxes/ubuntu_precise64_vbguest) v5.1.18
* upgraded base box version from 'v20170302.0.0' to 'v20170307.0.1'
* upgraded virtualbox guest addition to version 5.1.18
* performed apt-get update && apt-get dist-upgrade && apt-get autoremove
