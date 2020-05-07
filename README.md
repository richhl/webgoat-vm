#webgoat-vm

This Virtual Machine setup for WebGoat - WECARE LTD. uses  ***VagrantUP Virtual Machine*** to download Ubuntu and install Tomcat Server and the WebGoat application. It's ready for practicing penetration testing once booted within minutes!

When the virtual machine boots, WebGoat and it's dependancies are installed and ready to play with on:

http://127.0.0.1:50000/WebGoat


### What is VagrantUP

[VagrantUp](https://www.vagrantup.com/) is a pretty cool piece of virtualization software that allows you to spin up virtual machines from a command line and install software on them from a configuration file.

##Installation

### Prerequisites

You will need to install the following software:

- Install [git](http://git-scm.com/book/en/v2/Getting-Started-Installing-Git) to allow you to pull down the code from GitHub Code Repository
- Install VagrantUp on your system, see [VagrantUp](https://docs.vagrantup.com/v2/installation/)
- Install  VirtualBox, a free, cross-platform consumer virtualization product.
[Virtualbox](https://www.virtualbox.org/)

### Install WebGoat on a Virtual Machine

``` bash
git clone https://github.com/richhl/webgoat-vm.git
cd webgoat-vm
vagrant up

```

##Usage

When Vagrant has run, WebGoat will be installed on a virtual machine and accessible through port 50000

Goto the following URL to

```
http://127.0.0.1:50000/WebGoat
- Username: guest
- Password: guest
```

### Reset the Virtual Machine

The great thing about VagrantUP is that if you mess up, you can start again. Use the commands below to destroy the VM instance and re-provison it.

```bash
vagrant destroy
vagrant up
```
