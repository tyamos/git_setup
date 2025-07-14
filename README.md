# My documentation for GIT and GITHUB, beginners guide to setting up GIT and GITHUB. 


## 1. What is Version Control? 


Version Control is a system built to manage and keep record or track of documents overtime. 


## 2. What is Version Control used for? 

Version Control is best used for collaboration. 

## 3. What is GIT?

GIT is a version control system that is free and open source distributed. 

## 4. What is GITHUB? 

GITHUB is a platform that leverage Git for version control, primarily used by developers or engineers for collaborative work. 

## 5. Dfference between GIT and GITHUB. 
GIT: iS distributed version control system for keep record and updates in source code during any software development.
GITHUB: This is a web based hosting service, particularly for GIT, which offers a distributed version control and source code management. 

## 6. Comprehensive GIT and GITHUB setup on Linux Operating system for beginners. 

Before you install git, you first of all need to check if it is already installed on your device or not. By using the command "git --version", on a linux ubuntu operating system, it checks for any existing installations. 

If you run the code and Git is already installed, it will likely print a message that reads so, "git version 2.34.1". This means that git is already installed. For me, git was not installed on my device, X1 Carbon so I had to install it myself. So when I run the code to check if it exists or not, it echoed back to me that "git: command not found". 

To install Git on my device, I did the following:

Step 1: I ran the "sudo apt update" command. This command typically updates the system. 

Step 2: To install Git, I used the "sudo apt install git" command. This showed me some processing and required that I enter a "yes" to continue. 

Step 3: After the installation process was done, I used the command "git --version" to check if it was installed or not, and which version was installed.

Now to configure Git with your name and email, It was a bit of a tousle as I battled in my mind how to do it, but my tutor Bankat did justice to it and it somewhat felt easy. 

Step 4: So to make your details get registered, you use the command 'git config --global user.name tyamos' and then press enter. Please note that the "tyamos" I have used is my own name and you should use your own name. 

Step 5: After the name, next is your email, to register your email, you use the command "git config --global user.email august@gmail.com", and when you hit the enter key, it will save your record, but if you have doubts, you proceed to use the command "git config --list" to check if your details are registered. Booop! Your Git is set. 

We are now done with Git installationa and we will head to GitHub. 

To create an account, you head to the website  "https://github.com" and register with your active email and phone number. It is adviced that you use a professional email and not register with akward names like "Mhiz Prettiest" or "Don Handsome". You set your password and complete your registration by verifying through your registered email. 

If you are not familiar with Bash, then you need to get a teacher or get yourelf working to be better at it. Because I am not teachinng that. So let's proceed. Now that your Git and Github are set, we will now learn how to generate SSH keys to connect or link your Git and Github. 

Step 6: Your run the code "ls -al ~/.ssh".
Step 7: You run the next code which is "ssh-keygen -t ed25519 -C august@example.com" then you press enter. It will require you to set up a passphrase, kindly do not set the passphrase and press enter instead, it will ask you to verify, press enter again and it will be set. 

Step 8: "cat ~/.ssh/id ed25519.pub", use the command and when it executes, copy the oupout. Move to your Github,navigate to settings, locate SSH and GPG Keys, click on New SSH Key. Paste the key and name it, for me, I named mine after my laptop name, you can do same or find a better name. 

Step 9: Use the command "ssh -T git@github.com" to test the connection or link, it should display a message that it is successful if you followed all instructions above. 


I guess I have you time you should have gone back and forth to make this work. So, go ahead and push your lines to thw world! 

