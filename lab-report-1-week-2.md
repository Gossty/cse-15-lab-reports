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

**Note** You might get an "authenticity of host..." message. It's fine, you just need to type "yes" there.

## Trying Some Commands

Now we will try some commands:

* cd – change directory; if we type in just cd it will go to home directory, cd 'name' - goes to other directory;
* ls – shows a list of files and directories in the given directory 
* ls -a – list of files and directories in the given directory including hidden files (that start with ".");
* mkdir 'name' – creates a directory with a given name. 

Here is approximately what you should get:

![Image](Trying-Some-Commands.png)


