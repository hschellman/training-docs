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

   

{%include links.md%} 

[HSF Training Center]: https://hsf-training.org/training-center/   
[SL7_to_Alma9]: https://wiki.dunescience.org/wiki/SL7_to_Alma9_conversion#SL7_to_Alma_9_conversion
[indico-event-page]: https://indico.fnal.gov/event/59762/
[indico-event-requirements]: https://indico.fnal.gov/event/59762/page/3229-requirements
[dune-collaboration]: http://collaboration.dunescience.org/
[computing-account-request-form]: https://fermi.servicenowservices.com/com.glideapp.servicecatalog_cat_item_view.do?v=1&sysparm_id=d361073881218500bea3634b5c987c4c&sysparm_link_parent=a5a8218af15014008638c2db58a72314&sysparm_catalog=e0d08b13c3330100c8b837659bba8fb4&sysparm_catalog_view=catalog_Service_Catalog 
[get-connected-user-access]: https://get-connected.fnal.gov/users/access/ 
[kerberos-password]: https://fermi.servicenowservices.com/kb_view.do?sysparm_article=KB0011294 
[kerberos-template]: https://authentication.fnal.gov/krb5conf/ 
[kerberos-config]: https://fermi.servicenowservices.com/kb_view.do?sysparm_article=KB0011315 
[dunegpvm-status]: https://fifemon.fnal.gov/monitor/d/000000004/experiment-overview?orgId=1&var-experiment=dune&from=now-6h&to=now-5m&panelId=30&fullscreen
[dunegpvm-vnc]: https://wiki.dunescience.org/wiki/DUNE_Computing/Using_VNC_Connections_on_the_dunegpvms
[proxy-info]: https://cdcvs.fnal.gov/redmine/projects/sbndcode/wiki/Get_a_certificate_proxy 
[dune-setup-jan2021]: https://wiki.dunescience.org/wiki/DUNE_Computing/Setup_Jan2021
[dune-training-may2021]: https://dune.github.io/computing-training-202105/
[dune-wiki-interactive-resources]: https://wiki.dunescience.org/wiki/DUNE_Computing/DUNE_Interactive_Computing_Resources
[anaconda-faq-kinit]: https://github.com/DUNE/FAQ/issues/22
[dunefaq]: https://github.com/DUNE/FAQ

