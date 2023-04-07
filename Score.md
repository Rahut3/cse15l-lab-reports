# Remote Access 
---

In this post I will be showing you how I installed [Visual Studio Code](https://code.visualstudio.com/) then how I remotely connected using Visual Studio Code, then finally showing some commands to use in the terminal.
## Getting Your CSE15L Account

I got my CSE15L account by simply go to this [website](https://sdacs.ucsd.edu/~icc/index.php) and filled in my username and PID.
To reset my password I followed the links that told me to reset my password once I was in the website.


## Installing Visual Studio Code
First I went to the [Visual Studio Code](https://code.visualstudio.com/) website.
> If the link doesn't, copy and paste this into your browser: https://code.visualstudio.com/

![Image1](https://github.com/Rahut3/cse15l-lab-reports/blob/main/Visual-Studio-Code-1.png?raw=true)

I clicked on the download button to download. If you want to select your operating system, click on the arrow down to reveal more downloads for differen't systems.

![Image2](https://github.com/Rahut3/cse15l-lab-reports/blob/main/Visual-Code-2.png?raw=true)

After I have installed it and open it, its all set!

## Remotely Connecting

To remotely connect, I would first need to have Visual Studio Code open.
Then I would open up the terminal.

> Install [git](https://git-scm.com/) if your operating system is Windows 

> For my MacOS it would look like this:
> ![Image3](https://github.com/Rahut3/cse15l-lab-reports/blob/main/Screenshot%202023-04-06%20at%207.25.38%20PM.png?raw=true)

I clicked on the terminal and select new terminal.

With my terminal opened up I would then need to type:
`$ ssh cs15lsp23xx@ieng6.ucsd.edu`
Replacing the x's with the corresponding letters in your username. Then type in `yes` as an answer to the question that pops up. Then you would enter your password that you resetted, 
![Image4](https://github.com/Rahut3/cse15l-lab-reports/blob/main/Screenshot%202023-04-06%20at%2011.28.20%20PM.png?raw=true)

**Its done!**

## Commands

Now I can try some commands in the terminal!
```
Some key commands are:
ls
pwd
cd
```
cd (path goes here)  | Changes the working directory 
pwd                  | Displays the current working directory 
ls (path goes here)  | Can show me the files and folders in the given path determined by the directory 

