---
title: "Command Prompt: Basic Commands You Should Know (cmd)"
date: 2021-10-18T09:57:01+02:00
description: "A quick guide to basic cmd commands"
categories:
- Skill
- Code
tags:
- command prompt
keywords:
- tech
thumbnailImage: https://cdn.educba.com/academy/wp-content/uploads/2019/05/What-is-CMD.jpg
thumbnailImagePosition: left
metaAlignment: center
---

In Windows, when you open a command prompt, almost always the program that is running is cmd.exe. It's an enhanced NT derivative of the old DOS-based command.com, which is in turn has similarites with the even older CP/M CCP command interpreter.<!--more-->

In Linux, usually you are running bash in some sort of terminal emulator if you are using it in a graphical environment. (which can vary widely depending on your distro and desktop environment). This stands for "Bourne Again Shell" because it's an extended version of an earlier "Bourne" shell (sh)[^shell]: that's been standard on Unix for a long time. There's other "alternative" shells in common use such as csh, ksh, and tcsh.
[^shell]: Shell is a UNIX term for the **interactive user interface** with an operating system. The shell is the **layer of programming** that understands and executes the commands a user enters. In some systems, the shell is called a **command interpreter**. A shell usually implies an interface with a command syntax (think of the DOS operating system and its "C:>" prompts and user commands such as "dir" and "edit").

As the outer layer of an operating system, a shell can be contrasted with the kernel, the operating system's inmost layer or core of services.
The Windows cmd.exe can be considered a shell as well (as can explorer.exe).

Both the Windows command prompt and all Unix shells have several "built-ins", or commands that are handled entirely within the shell. This includes some basic commands (such as cd) and many conditional commands and operators that control script flow if a batch file of commands are executed.

However, in both Linux and Windows, the great majority of "commands" that do useful things are in fact external programs that are "called" by the the shell. And that is the primary purpose of a shell, to enable an operator to start programs with specifying arguments for those programs. It's not really strictly a programming language, it's just a framework for launching programs.
<!--more-->
{{< toc >}}
### Change the Directory / Folder (cd)/ Drive
Use `cd \` to {{< hl-text red >}}go to the top of the directory tree{{< /hl-text >}}.

If you need to {{< hl-text red >}}go to a specific folder{{< /hl-text >}} from this drive run the command CD Folder. The subfolders must be separated by a backslash character: `\`.

Use the `cd..` command to {{< hl-text red >}}go one folder up{{< /hl-text >}}.

If you wanted to {{< hl-text red >}}change the drive{{< /hl-text >}} from “C:” to “D:”, type `d:` and then press `Enter`.

### Create a New Directory / Folder (mkdir)

You can {{< hl-text red >}}make a new folder{{< /hl-text >}} using the `mkdir <your folder name>` (Make Directory) command. The syntax of these commands is mkdir Folder.

{{< hl-text red >}}To test{{< /hl-text >}} if it worked, use the `dir` command. The newly created folder appears in the list.

If you are working on the “C:” drive and you want to {{< hl-text red >}}create a new folder in another Drive{{< /hl-text >}} D called "Google", type `mkdir d:\Google` and then press `Enter`.

### Clear Screen (cls)
To clear the existing commands in prompts type `cls` and press `Enter`.

### Run software
To run software in cmd, Put your shortcuts or .exe (executable file) in the current path where you can `start <softeare name>`
{{< alert info >}} You can directly type the system names (not shortcut names) {{< /alert >}}
Common program names include the following:
{{< hl-text red >}}File Explorer{{< /hl-text >}}: `explorer`
{{< hl-text red >}}Task Manager{{< /hl-text >}}: `taskmgr`
{{< hl-text red >}}Character Map{{< /hl-text >}}:`charmap`
{{< hl-text red >}}Advanced System Properties{{< /hl-text >}} (for Path setting):`systempropertiesadvanced`
{{< hl-text red >}}My Computer{{< /hl-text >}}:`explorer =` or `explorer /root,`
**{{< hl-text red >}}Control Panel{{< /hl-text >}}**:`control`


### Lists Installed Drivers (driverquery)
Drivers are very important in your PC. Missing a important driver can hamper your work. Use `driverquery` command to get a full list of installed drivers in your pc. It’ll help you to find the missing driver.

### Networking Information (ipconfig)
`ipconfig` will provide you your ip address along with your local network.

### List Hardware Information (systeminfo)
Use `systeminfo` to know very basic information about your pc’s hardware, like – motherboard, processor & ram.

### Check if Server is Reachable (ping)
The ping command sends packets of data to a specific IP address (or domain) on a network and then lets you know how long it took to transmit that data and get a response.
pin
If you get the response properly then the connection of the device is working properly if not a particular server or your online connection is blocking communication between your computer and another.
`ping <ip or domain>`

### Scan and Repare System Files (sfc /scannow)
`sfc /scannow` will scan and repare windown system files. But you must be run the console as an administrator.

### List Currently Running Tusk (tasklist)
Use `tasklist` to get currant list of all tasks running on your pc.


S
