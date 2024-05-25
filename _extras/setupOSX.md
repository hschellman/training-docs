---
title: OSX setup
teaching: 60
exercises: 0
questions:
- How do I set up a mac to run root and other HEP software
objectives:  
- Get ready to do the tutorial
- Set up your computing environment in an apple system
- Set up grid access and job submission
keypoints:
- You need a compiler and a version control system to get started
---
## Objectives


## Requirements


> ## Note

## Instructions by OS

These are instruction to get a compiler on your local system.

[Apple computers]({{ site.baseurl }}/setupOSX).

## 3. Get a clean shell
To run HEP software, it is necessary to have a 'clean environment'. What is meant by clean here? 

Two ways to clean your shell once.

**Cleanup option 1:** Manual check and cleanup of your custom environment variables
To list all of your environment variables:

~~~
env
~~~
{: .language-bash}

The list may be long. 

Once you identify environment variables that might conflict with your work, you can tweak your login scripts, like .bashrc, .profile, .shrc, .login etc., to temporarily comment out those (the "export" commands that are setting custom environment variables, or UPS's setup command).  Note:  files with names that begin with `.` are "hidden" in that they do not show up with a simple `ls` command.  To see them, type `ls -a` which lists **a**ll files.

**Cleanup option 2:** Back up your login scripts and go minimal at login (recommended)

A simpler solution would be to rename your login scripts (for instance .bashrc as .bashrc_save and/or .profile as .profile_bkp) so that your setup at login will be minimal and you will get the cleanest shell. For this to take into effect, you will need to exit and reconnect through ssh.

> ## How to make custom setup command with aliases
> Not familiar with aliases? Read below.
> 
> To create unix custom commands for yourself, we use 'aliases':
> ~~~
> alias my_custom_commmand='the_long_command_you_want_to_alias_in_a_shorter_custom_name'
> ~~~
> {: .source}

> For DUNE setup, you can type for instance:
> ~~~
> alias setup_root='activate myroot_env'
> ~~~
> {: .language-bash}
> 
> So next time you type:
> ~~~
> doroot
> ~~~
> {: .source}
> Your terminal will execute the long command. This will work for your current session (if you disconnect, the alias won't exist anymore). You can store this in your (minimal) .bashrc or .profile if you want this alias to be available in all sessions. The alias will be defined but not executed. Only if you type the command `doroot` yourself.
{: .solution}

Try testing ROOT to make certain things are working


### Useful Links
[HSF Training Center][HSF Training Center]
   

{%include links.md%} 

[HSF Training Center]: https://hsf-training.org/training-center/   


