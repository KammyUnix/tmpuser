![TMPUser demo](assets/tmpuser.gif)
# TMPUser

when you don’t wanna mess up your home directory, but you’re too lazy for containers or VMs.
<p align="center">
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white" alt="Bash" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux" />
  <img src="https://img.shields.io/badge/fzf-required-blue?style=for-the-badge" alt="fzf required" />
  <img src="https://img.shields.io/badge/License-GPL--3.0-blue?style=for-the-badge" alt="GPL-3.0" />
</p>

## wat is this?

tl;dr: **temu docker/podman**

TMPUser basically makes your home directory temporarily live in `/tmp`, making other apps think:

> “ah yes, my user’s home directory is `/tmp`. average classic day.”

think of it like chrooting into `/tmp`, but kernel and users and etc stay same, except path and home directory variables

unless.. you just use it to create `/tmp/$user` directory and don't use the main feature of TMPUser. what a psychopath?!

## how does it work?

tl;dr: **magic**, okay just joking, my bad.

basically, it temporarily changes every path to new created "workspace" (aka, directory in your `/tmp` that you created using tmpuser), 

so yes, if you have custom binaries in your `/home`, it wont work there(but you can carry over any files)

## installation

grab latest version in releases(if i’ll ever update lol)

`curl -LO https://github.com/KammyUnix/tmpuser/releases/download/v1.0.0/tmpuser.tar.gz`

then extract it

`tar -xzf tmpuser.tar.gz`

and use it!

`./tmpuser`

**optionally, you can add to PATH**

## known issue

![error picture n1](assets/error%20n1.jpeg)

i am too lazy to fix, ignore while hopefully after 10 years, i’ll fix this

## contributing

this shit is held together with tapes and hope, and probably has hundreds of security holes

please, if you can, make this code better🙏
