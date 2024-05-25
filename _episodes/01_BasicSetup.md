---
title: Basic Setup - tested on OSX
teaching: 30
exercises: 0
questions:  
- How do I get started in scientific programing
objectives:  
- Learn how to use command line tools
- Install software you need to do scientific programing
keypoints:
- This will be useful for a lot of projects
- It is also something almost all people who get paid to program are expected to know well
---

## 1. Back up your machine

We are going to be messing with your operating system at some level so it is extremely wise to do a complete backup of your machine to an external drive right now. 

Also turn off automatic updates.  Operating system updates can mess with your setup.  Generally, back up before doing updates so you can revert if necessary. 

## 2. Learn how to do a terminal session and use the Unix Shell

There is a nice tutorial from the Carpentries at: [Unix Shell Basics][Unix Shell Basics].
It tells you how to start a terminal session in Windows, Mac OSX and Unix systems. 

Please do the shell tutorial to learn about the basic command line. 

## 3. Install some basic tools

You are going to need to add some package to your local machine

### 1. Install Git

Github is a repository for shared code.  It is also a good place to back up your code and share with others.  You will need to set up an account if you want to store things there. 

Start out by doing the setup/install section of the tutorial at [https://swcarpentry.github.io/git-novice/](https://swcarpentry.github.io/git-novice/) to get started.  You can come back and do the full tutorial later. 

### 2. Get a compiler/code editor

Although you will mainly be using python to code to begin with, most HEP code is actually C++ and it is good to have access to a C++ compiler.  Bonus is that you normally get a good editor as well. 

#### OSX
On OSX, you should install [Xcode][Xcode] from the [App store](https://www.apple.com/app-store/).  It will take a lot of disk space. When you try to use it it will ask you to install command line tools.  Do so. 

Even though Xcode is what you use to compile and has an editor, many people prefer to use the [Visual Studio Code](https://code.visualstudio.com) application from Microsoft for editing/testing code. 

#### Unix
Your compiler will be gcc 
Heck - just use vim. Or emacs, or [VSCode][Visual Studio Code].

#### Windows 
Likely you should load up the full Visual Studio as it has a nice C++ compiler

### 3. Install an x-windows emulator

#### OSX
Install [XQuartz][XQuartz]  

test it out by typing

~~~
xterm &
~~~
{: .language-bash}

You should get a terminal window. You can close it. 

#### Unix 
Already have one

test by doing 

~~~
xterm &
~~~
{: .language-bash}

### 4. Install Conda

See [Next lesson]({{ site.baseurl }}/_episodes/02_InstallConda.md)











### Useful Links
[HSF Training Center][HSF Training Center]

[Unix Shell Basics][Unix Shell Basics]   

[Visual Studio Code][Visual Studio Code]

[Visual Studio][Visual Studio]

[GNU gcc][GNU gcc]

[Xcode][Xcode]

{%include links.md%} 

[HSF Training Center]: https://hsf-training.org/training-center/   
[Unix Shell Basics]: https://swcarpentry.github.io/shell-novice/
[Visual Studio Code]: https://code.visualstudio.com
[Visual Studio]:https://visualstudio.microsoft.com/vs/
[GNU gcc]: https://gcc.gnu.org]
[App Store]: https://www.apple.com/app-store/
[Xcode]: https://developer.apple.com/xcode/
[XQuartz]: https://www.xquartz.org

