# Homeworks

## Guide

- Each group MUST create a Pull Request to this repo, with a file named `Answer.md` inside this `Homeworks` folder.
- Set the Pull Request name as your Group name. For example: `Group 1`
- Write out your Group's members and other notices in the Pull Request description.
- Write out steps and commands that you made to complete each homework in the answer file.

## Homework 1

- Find the `rpm` commands (if exists) which has the same funcionality with `dpkg` commands listed [here](../ex01_Install_Packages#working-with-dpkg)
- Find the `yum` commands (if exists) which has the same funcionality with `apt` commands listed [here](../ex01_Install_Packages#working-with-apt)

## Homework 2

Convert **rpm** package of `bless` to **deb** package and install. Source: https://www.rpmfind.net/linux/rpm2html/search.php?query=bless

## Homework 3

Create an alias command that list 5 files that is last modified in a folder

## Homework 4

Add Ubuntu code name to prompt. Example: Ubuntu 14.04 is `trusty`. Get code name from `/etc/lsb-release`, do not hardcoded it !

```
{trusty}root@d62797bc75eb:/#
```

## Homework 5

Create an alias command `kill_all` that kill all processes that match `{search_phrases}`.

Ex: `kill_all bash`, `kill_all gedit`

## Homework 6

Create an alias command `gplo` that is same as `git pull origin {current_branch}` (we don't have to input current branch name)
