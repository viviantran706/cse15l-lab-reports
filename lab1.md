# Lab Report 1

## Step 1- Downloading Visual Studio Code (VSC)
(If VSC is already downloaded skip this step)
Otherwise, go to the VSC website
[Link](https://code.visualstudio.com/), go thorugh the downloading instrustions and 
download the apporiate system according to desktop, like Mac and Windows.

When it has installed, open the file. Then, a new window should appear on your screen.
(The coloring and placement can differ according to the changes that are made in the
preference settings. The files that pop up on the picture below might ): 

![Image](https://raw.githubusercontent.com/viviantran706/cse15l-lab-reports/main/Screenshot%202023-04-06%20121847.png)

## Step 2- Remotely Connecting 
Start off by installing Git: [Link](https://gitforwindows.org/)

Go thorugh the downloading processes.

We will also need Bash in VSC: [Link](https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal/50527994#50527994)

Go through the steps to download.
Find your username thorugh: [Link](https://sdacs.ucsd.edu/~icc/index.php)

And you should see `cs15lsp23zz` (the zz will be replaced by your specific letters). Click that then click the Global Password change Tool then Proceed to the Password Change Tool. Then when entering your username to reset the password make sure to enter the username we just found **rather then the username to you ucsd email**


If the terminal is not open already, follow these steps to open in:
1. In the menu bar, there should be a part called terminal
2. Hover over and go to "New Terminal" (or hold Ctrl + shift + `)
3. In the terminal, make sure you are in the bash terminal. To ensure this click the drop down arrow. And click Git Bash.
4. In the terminal, enter `ssh cs15lsp23zz@ieng6.ucsd.edu` in the terminal. Replace the zz with the las two letters in you username (can be found at [Link](https://sdacs.ucsd.edu/~icc/index.php).)

When the message `Are you sure you want to continue connecting (yes/no/[fingerprinit])?` Print yes then enter. Then the next question to answer is **Password**, print and enter the information.

If you see this photo below, then you know you have done the steps correctly.

![Image](https://raw.githubusercontent.com/viviantran706/cse15l-lab-reports/main/Screenshot%202023-04-06%20123418.png)

## Step 3- Running some Commands
Now after step 2, in the terminal there are a few commands that we will run, with a quick run down on each command:

-cd (This is the command to change the current directory)

-ls -lat (This command produces files form the home directory)

-ls -a (This command prompts all the files and directoroies)

-ls <directory> where <directory> is /home/linux/ieng6/cs15lsp23/cs15lsp23abc, where the abc is one of the other group members’ username (This command displays what other files the directory)

-cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/ (This command takes the user to the hello.txt file)

-cat /home/linux/ieng6/cs15lsp23/public/hello.txt (This command prints the hello.txt in the terminal).

---

Here is an exmaple of what the command -ls -a should print 
  
![Print](https://raw.githubusercontent.com/viviantran706/cse15l-lab-reports/main/Screenshot%202023-04-06%20125122.png)
  
  

  
If you are done with these commands to exit: Crtl-D or run the command `exit`.
