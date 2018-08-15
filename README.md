# Virtualization made easy

Vagrant from HarshiCorp is a very powerfull virtualization orchestrator. In this simple example we run a `Windows Server 2016 Standard 1607` VM in `Virtualbox` on `MacOSX`.

## Prerequisites
You will need to have both [Vagrant](https://www.vagrantup.com/intro/index.html) and [Virtualbox](https://www.virtualbox.org/) installed on your system. If you don't you can use the following commands to install them.

> Please note that you will require Homebrew to run the commands, if you don't have it installed follow this [link](https://brew.sh/)

**Install Virtualbox**
```bash
$ brew install cask virtualbox
```
**Install Vagrant**
```bash
$ brew install cask vagrant
```

## Setting up

You now have access to the most easy to use VM orcherstrator I personally have come across thus far. Vagrant allows you so set up virtual machines on any VM service provider like Oracle Virtualbox on Mac/Linux/Ubuntu and HyperV on Windows systems.

The instructions for setting up are as follows:

1. In your working directory of choice, clone the repo
```bash
$ git clone https://github.com/indungu/windows-server-on-mac.git
```
2. Launch the box
```bash
$ vagrant up
```

