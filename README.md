# PDQ Chaos Koala Watcher

## Instructions
Here at PDQ.com we pride ourselves on being at the **very** cutting edge of technology. When we heard that Netflix created a *Chaos Monkey* program (https://github.com/Netflix/chaosmonkey) to introduce faults in their systems, we didn't want to be out done. So, we created our own *Chaos Koala* to randomly change files on our network. Unfortunately, we forgot to check these file changes and report back to our corrective systems. As a next step and part of our hiring process for this specific role, we ask that you write an application to address this problem.  **(If you are unable to complete this step, our process will not allow us to consider your application.) **

**NOTE BEFORE YOU BEGIN**: Please treat this assignment as you would treat any other production code -- take your time and do it right. Other talented programmers have failed by not taking this advise. This is not a timed assignment. We are aiming to assess what you would submit as production code. Use C# to implement the project. Zip up your implementation sources into a single file. When you submit your resume to PDQ, you will get an email directing you to the URL to upload your submission. Or, you can post your submission to a public git repository and let us know where to find it.

## Assignment
The *Chaos Koala* is busy creating and modifying text files in some specific directories. We want you to create a command-line program to watch a directory we provide. The program should detect files created or modified and then output information about them. We strongly suggest creating some sample files of various sizes and testing your program for performance before submitting. 

* The program takes 2 arguments, the directory to watch and a file pattern, example: program.exe "c:\file folder" *.txt
* The path may be an absolute path, relative to the current directory, or UNC.
* Use the modified date of the file as a trigger that the file has changed.
* Check for changes every 10 seconds.
* When a file is created output a line to the console with its name and how many lines are in it.
* When a file is modified output a line with its name and the change in number of lines (use a + or - to indicate more or less).
* When a file is deleted output a line with its name.
* Files will be ASCII or UTF-8 and will use Windows line separators (CR LF).
* Multiple files may be changed at the same time, can be up to 2 GB in size, and may be locked for several seconds at a time.
* Use multiple threads so that the program doesn't block on a single large or locked file.
* Program will be run on Windows 10.
* File names are case insensitive.

# Review Instructions
1. Create a github repo.
2. Write code.
3. Send us an email with the URL of your repo.
