---
toc: true
comments: true
layout: post
title: Download and Setup Tools
description: Download and setup instructions for all the tools
courses: { compsci: {week: 0} }
type: hacks
---

## Hacks
> Complete the procedure below accurately. DO NOT SKIP STEPS.

### GitHub Account
- Follow instruction [https://docs.github.com/en/get-started/signing-up-for-github/signing-up-for-a-new-github-account](https://docs.github.com/en/get-started/signing-up-for-github/signing-up-for-a-new-github-account). Use personal email because this GitHub account belongs to you.

### Windows
> VSCode install using WSL. Windows users have option to have best of Windows and Linux while developing within VSCode.
- Install [VSCode using WSL]({{site.baseurl}}/techtalk/vscode-wsl).
- Required review, become familiar with [Windows WSL development](https://code.visualstudio.com/docs/remote/wsl-tutorial)
- Or google VSCode download and that works too
- Install the extensions: Python, Jupyter Notebooks, Remote Explorer, WSL, and all other ones that come with it

> Install WSL
- [Download WSL](https://learn.microsoft.com/en-us/windows/wsl/install) and follow instructions

> Install Docker
- [Download Docker](https://docs.docker.com/desktop/wsl/#:~:text=With%20Docker%20Desktop%20running%20on,to%20improve%20the%20resource%20consumption.) and follow instructions

> Install Jupyter Notebooks
- Run:
```bash
(base) id:~$ sudo apt-get install jupyter-notebook
(base) id:~$ jupyter kernelspec list # list installed kernels
```
> Setup
- Go to home directory and run:
```bash
(base) id:~$ mkdir vscode
(base) id:~$ cd vscode
(base) id:~$ git clone https://github.com/nighthawkcoders/teacher.git
(base) id:~$ git config --global user.email <your email without the <>>
(base) id:~$ git config --global user.name <your github id without the <>>
```
- Use student template and create student repository and copy HTTPS link provided
- Run:
```bash
(base) id:~$ git clone <link copied without the <>>
```
- To install other tools, run installation script:
```bash
(base) id:~$ ~/vscode/teacher/scripts/activate_ubuntu.sh
```
- To check versions, run:
```bash
(base) id:~$ ruby -v
(base) id:~$ python --version # should be 3.9 or better
(base) id:~$ jupyter --version # should see nbconvert
(base) id:~$ jupyter kernelspec list # should see python3
```
- To open blog, run:
```bash
(base) id:~$ bundle install
(base) id:~$ make # always run make clean after closing it
```

> Anaconda install on WSL (NOTE: Anacoda likely not used this year, so skip these steps)
- Try the exact commands in WSL Command / Powershell.  
- Only if there is a wget error... To find the latest Linux-x86 distribution hover over ```64-Bit (x86) Installer``` of this page: https://www.anaconda.com/download#downloads.  Hover over  wget and Anaconda3 commands based on new link.
```bash
> PS C:\Users\UserName> wsl  # Windows prompt to WSL command
$ cd /tmp
$ wget https://repo.anaconda.com/archive/Anaconda3-2023.03-1-Linux-x86_64.sh
$ chmod +x Anaconda3-2023.03-1-Linux-x86_64.sh
# Answer yes to all the prompts
$ ./Anaconda3-2023.03-1-Linux-x86_64.sh
```

> At this point, the next task is to prepare for Packages, Jupyter Notebooks, and Kernels.  <mark>You must start a new WSL Command / Powershell</mark>.  Now the WSL prompt should be <mark>prefixed with (base)</mark> from Anaconda install.  If not, you need to go back to Anaconda install.
- Open Command / Powershell.  If you are not looking like this you need to back up.
```bash
> PS C:\Users\ShayM> wsl  # Windows prompt
(base) shay@MSI:/mnt/c/Users/ShayM$ cd ~ # WSL prompt
(base) shay@MSI:~$ # WSL home, best place to install files
```

> Key Packages needing update on WSL Ubuntu
- In a WSL Command / Powershell install Python3
```bash
$ sudo apt list # list packages
$ sudo apt update # update package list
$ sudo apt upgrade # upgrade packages
$ sudo apt install python3 python3-pip # install python3 and pip3 for development
$ python --version  # version of python3 should be shown