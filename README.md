# Virtualization made easy

Vagrant from Hashicorp is a very powerfull virtualization orchestrator. In this simple example we run a `Windows Server 2016 Standard 1607` VM in `Virtualbox` on `MacOSX`.

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
3. Once this is complete, and it might take a while since the box is rather large, you can access it via the virtualbox UI. 
```bash
$ Virtualbox # To launch the ui
```
> select the virtual machine whose name starts with the name of your working directory followed by `_default_*` where the wildcard is a random intenger value. It's status should be `running`.

4. Click the `Show` button to view the VM's GUI.

![image](https://user-images.githubusercontent.com/30072633/44178992-7b43a180-a0fd-11e8-9221-87b1db104458.png)


### Side note
The Windows Server Standard installed is unlicensed but it does come stacked with some cool features. You can configure it further with Windows [PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6).
For more on what the box come with, you can check out the maintainer's notes on Vagrantcloud [here](https://app.vagrantup.com/gusztavvargadr/boxes/w16s)
