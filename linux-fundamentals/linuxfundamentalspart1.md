# Linux Fundamentals Part 1
Embark on the journey of learning the fundamentals of Linux. Learn to run some of the first essential commands on an interactive terminal.

## Task 1: Introduction
**Let's get started!**

> Answer: No answer needed

## Task 2: A Bit of Background on Linux
**Research: What year was the first release of a Linux operating system?**

Search on Google.

> Answer: 1991

## Task 3: Interacting With Your First Linux Machine (In-Browser)
**I've deployed my first Linux machine!**

> Answer: No answer needed

## Task 4: Running Your First few Commands
**If we wanted to output the text "TryHackMe", what would our command be?**

*echo* command is used to show some text in the output.

> Answer: echo TryHackMe 

**What is the username of who you're logged in as on your deployed Linux machine?**

Deploy the machine. Type *whoami* command to view username.

> Answer: tryhackme

## Task 5: Interacting With the Filesystem!
**On the Linux machine that you deploy, how many folders are there?**

*ls* command is used to view files and directories list.

> Answer: 4

**Which directory contains a file?**

*ls* command is used to view files and directories list. The *ls foldername* command is used to check files inside a folder. After giving *ls folder4* command, we can see a file. ie there are files in folder4. Also check inside each folder using *cd* command. 

> Answer: folder4

**What is the contents of this file?**

The *cat* command is used to view the contents of a file in the output.

> Answer: Hello World

**Use the cd command to navigate to this file and find out the new current working directory. What is the path?**

First use *cd folder4* command to enter folder4. Then type *pwd* command to view the current working directory.

> Answer: /home/tryhackme/folder4

## Task 6: Searching for Files
**Use grep on "access.log" to find the flag that has a prefix of "THM". What is the flag?**

Type *grep "THM" access.log* to find the flag. You can also find the flag using *cat access.log | grep "THM"* command.

> Answer: THM{ACCESS}

**And I still haven't found what I'm looking for!**

> Answer: No answer needed

## Task 7: An Introduction to Shell Operators
**If we wanted to run a command in the background, what operator would we want to use?**

> Answer: &

**If I wanted to replace the contents of a file named "passwords" with the word "password123", what would my command be?**

The *>* operator is used to overwrite contents of a file.

> Answer: echo password123 > passwords

**Now if I wanted to add "tryhackme" to this file named "passwords" but also keep "passwords123", what would my command be**

The *>>* operator is used to add contents of a file.

> Answer: echo tryhackme >> passwords

**Now use the deployed Linux machine to put these into practice**

> Answer: No answer needed

## Task 8: Conclusions & Summaries
**I'll have a play around!**

> Answer: No answer needed

## Task 9: Linux Fundamentals Part 2
**Terminate the machine deployed in this room from task 3.**

> Answer: No answer needed

**Join [Linux Fundamentals Part 2!](https://tryhackme.com/room/linuxfundamentalspart2)**

> Answer: No answer needed

***Written by: Shariat Ullah Pathan***
