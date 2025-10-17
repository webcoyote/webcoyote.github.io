# Webcoyote.github.io

**Patrick Wyatt's GitHub projects**

If you've looked at my [GitHub page](https://github.com/webcoyote) you might be a bit confused by all the projects listed there. What are they and how do they relate to each other?!? I hope this page will explain.

## Building Linux virtual machines

I have Mac and Windows laptops, but prefer developing web applications on Linux in virtual machines so I can simulate the environment those apps will be deployed on. Building virtual machines is time-consuming, so I've automated the process using several projects.

- [linux-vm](https://github.com/webcoyote/linux-vm): [Original] [Windows] Builds a complete Linux virtual machine including installing all required software ([VirtualBox](https://www.virtualbox.org/), [Vagrant](http://vagrantup.com/), [Chocolatey](http://chocolatey.org/), and [Git](http://git-scm.com/)). This project is designed to make it easy to test-drive Linux.

- [workstation-setup](https://github.com/webcoyote/workstation-setup): [Original] [Mac/Linux] After I've purchased a new computer or built a virtual machine, it always seems a bit empty. I use this project to specify the Mac/Linux software that I use regularly during developing, including my editor ([Sublime Text 2](https://www.sublimetext.com/), my shell ([Zsh](http://www.zsh.org/) and [Oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)), my browser ([Firefox](http://www.mozilla.org/en-US/firefox/new/)), my desktop window manager ([XMonad](http://xmonad.org/)), and other useful programs.

- [pivotal_workstation](https://github.com/webcoyote/pivotal_workstation): [Cloned] [Mac/Linux] This repo contains a large set of recipes used to install software. It was primarily used to configure Mac systems but I've been updating it to include more Linux recipes and make it work on CentOS as well as Ubuntu. This project is referenced by workstation-setup to perform the actual software installation work.

- [dotfiles](https://github.com/webcoyote/dotfiles): [Original] [Mac/Linux] Everyone likes to configure their software to their own special needs. This repository contains the settings I use for my projects. This project is referenced by linux-vm to install *my* dotfiles; you can clone it so that you can load *your* changes when you're building virtual machines.

- [veewee-berkshelf](https://github.com/webcoyote/veewee-berkshelf): [Cloned] [Mac/Linux/Windows] Builds virtual machine "base box" images for [Vagrant](http://vagrantup.com/) from Linux ISO files. If you don't trust others to build Vagrant boxes then you'll want to clone this recipe and build your own.

- [chef-solo-search](https://github.com/webcoyote/chef-solo-search): [Cloned] [All platforms] If you're using the [Chef] system provisioning platform for Vagrant, you'll discover many of the system configuration recipes require Chef Server. This repository makes it possible to utilize Chef without Chef Server. I modified the library to incorporate changes by another programmer for Chef 11, which haven't been accepted into the mainline yet.

- [chef-dotfiles](https://github.com/webcoyote/chef-dotfiles): [Original] [Mac/Linux] This repository is used by linux-vm to perform installation of "dotfiles" (configuration files) onto computers during the provisioning process.

- [chocolatey](https://github.com/webcoyote/chocolatey): [Cloned] [Windows] The Chocolatey package manager makes it possible to install software from the command line, or using a script, as I do in the [linux-vm install script](https://github.com/webcoyote/linux-vm/blob/master/INSTALL.ps1). I modified the library to add error-handling, which changes have not been accepted into the mainline yet.

- [chocolatey-packages](https://github.com/webcoyote/chocolatey-packages): [Original] [Windows] Scripts for the Vagrant package when using the Chocolatey package manager.

## Linux utilities

- [gnome-config-listener](https://github.com/webcoyote/gnome-config-listener): [Original] [Linux] This project is used to build a program that listens for [Gnome desktop](http://www.gnome.org/) configuration changes and writes them to the terminal. I can configure my computer and save all the changes so they can be replayed on other computers.

- [network](https://github.com/webcoyote/network): [Cloned] [Linux] A program that visualizes network traffic using 3d imagining. I added some scripts to install the pre-requisites and make the program run "nicely".

## Windows development

- [CSNamedPipes](https://github.com/webcoyote/CSNamedPipes): [Original] [Windows]
CSNamedPipes is a demo application that implements interprocess communication (IPC) using Named Pipes in C#. Many programmers had problems handling client-disconnects using Named Pipes, so I wrote this application to (a) learn C# and (b) solve that problem.

- [coho](https://github.com/webcoyote/coho): [Original] [Windows] This library is a basic toolkit for writing C++ programs from scratch on Windows. After having done this many times before I decided to open-source it so I won't have to rewrite again. Sadly most of my recent development has been on Linux and this library has languished.

## Obsolete

- [build-linux-vm](https://github.com/webcoyote/build-linux-vm): [Windows] This was an earlier attempt at building Linux virtual machines, but it requires too many manual steps!

- [linux-setup](https://github.com/webcoyote/linux-setup): [Linux] An earlier attempt at system configuration that has since been replaced by my workstation-setup and dotfiles repos.

- [vagrant](https://github.com/webcoyote/vagrant): [Cloned] [Windows] added SSH support for Windows [merged]
