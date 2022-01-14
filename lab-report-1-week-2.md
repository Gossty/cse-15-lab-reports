# Lab Report №1

This is a short tutorial on how to log into a course-specific account on ieng6.

## Installing VScode
The first step we are going to take is installing Visual Studio Code on our local computers. One can do it by using [this link](https://code.visualstudio.com/download). When you click the link you should see something like this:

![Image](VS-website.png)

After installing VS code and agreeing to appropriate license conditions, you should be able to open a window similar to the screenshot below:

![Image](VS-Installment.png)

Now we are ready to move on.

## Remotely Connecting

Since my laptop runs on Mac operating system I will cover the steps required for Mac users to connect to ieng6. Here are the steps: 
* open a terminal (hotkey shortcut: "control" + "shift" + "`" [a symbol next to shift])
* type in "ssh cs15lwi22ant@ieng6.ucsd.edu" (instead of "ant" you should have some other letters) and enter your Password.

If you do everything correctly, you should get the following output in a terminal:

![Image](SSH-login.png)

**Note**: You might get an "authenticity of host..." message. It's fine, you just need to type "yes" there.

## Trying Some Commands

Now we will try some commands:

* `cd` – change directory. If we type in just cd it will go to **home** directory;
* `cd <name>` - goes to other directory;
* `ls` – shows a list of files and directories in the given directory;
* `ls -a` – list of files and directories in the given directory including hidden files (that start with ".");
* `mkdir <nameOfFolder>` – creates a directory with a given name. 

Here is approximately what you should get:

![Image](Trying-Some-Commands.png)

**Note**: *There is a "Permission Denied" output in line 29 in screenshot, since I was trying to look into another students directory.*

## Moving Files with **scp**

The next thing we are going to do is moving local files from our **local** machine to **remote** ieng6. This can be done with the following line: `scp <FileName.java> cs15lwi22atn@ieng6.ucsd`.edu~/. You should get something like this:

![Image](SCP.png)

**Note**: *Don't forget to create a file on your local device first.*

At first when I ran WhereAmI file on my laptop, it showed me MAC OS X, my username, home directory and a path to download directory. After logging into ssh  OS changed to Linux and home directory changed to another. 

## Setting an SSH Key

Now we will set up an SSH key, so that log in process would take less time. Here are the steps you should take:
1. 