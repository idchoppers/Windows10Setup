Win10SetupScript.ps1
====================
Before you run!
Make sure that you are completely up to date. If you are not, then the restart will force an update and it WILL revert some changes.
Needs Admin privileges to run.
What it does:
* Makes a restore point
* Changes wallpaper to solid black
* Mutes all system sounds
* Adds an Open PowerShell here option
* Sets power to High Performance
* Makes UAC prompt for password to run a file with Admin privs
* Disables easy access stuff for keyboards (sticky keys, toggle keys, etc.)
* Unhides hidden files
* Shows file extensions
* Gets rid of OneDrive ad on explorer
* Disables Pretty Path
* Disables Aero Shake
* Makes explorer's default page This PC
* Hides taskbar clutter
* Makes taskbar use small icons
* Enables Dark mode
* Enables Aero theme
* Disables the "Swipe up to logon" thing on the lock screen
* Makes Winlogon use a solid color
* Make start menu appear faster
* Removes Bing search suggestions on start menu
* Removes "Look For App in App Store" option when opening a file with an unknown extension
* Disables Cortana
* Enables Secure Attention (Ctrl+Alt+Del) to logon
* Enables verbose mode
* Disables all animations
* Installs WSL2
* Prompts for restart
* Other cool stuff

When this is done running and you have restarted, run the WSLSetupScript 

WSLSetupScript
==============
This script should be ran after the reboot from the first script. It does not need elevated privs to run!
* Installs WSL kernel patch
* Enables WSL2
* Installs Debian
* Installs Windows Terminal
* Runs Debian for further configuration

When this is done everything for Windows should be set up and installed!

sounds.reg and openpshere.reg
=============================
Both of these files are large changes to the registry that will be imported by the script.

img0.jpg
========
A wallpaper that is just solid black. Very nice to look at and is not distracting at all.

DebianSetup.sh
==============
Setup script for Debian in WSL2, do not run with root, it will prompt when it needs it.
* Updates and upgrades
* Installs some programs
* Copies config files

After this is done you now have a completed environment!

.vimrc
======
My vimrc config

.bash_aliases
=============
My bash aliases and PS1
