# A-BEGINNERS-GUIDE-TO-GITBASH #
This article will introduce you to Gitbash and how to push and pull requests on git using gitbash.
------------------------------------------------------------------------------------------------------------------

![Git](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/1q8m7t23bpz9rdx1iv6g.png)


## **Are you a newbie on git like me?** ##


Check out this article on how you can install and configure Git also known as *gitbash* and connect it to your GitHub account on a Windows operating system, using commands and prompts.


<u>**Definitions:</u>**


 - **Github** - This is a virtual control platform that allows you to create, store, manage, track, and share your code with other developers. It enables collaborations on projects.

 - **Git/Gitbash** - This is a command-line version control interface that allows you to communicate with your GitHub account using prompts and commands. 


**Fun fact about git:**
> 
*Git uses the SHA-1 (and increasingly SHA-256) cryptographic hashing algorithm to identify every commit. This ensures that the code cannot be altered or corrupted without detection.*  



- **Commit** - Is a permanent record of your code at a specific point in time. A code checkpoint that can be secured using cryptography.


 
***Now that you know the tools, let's get started!***

#### How to Install GitHub Locally: ####

*Step 1:*
Open your default browser and search *github*, click the first link, and sign up. OR follow this link to [Github and sign up](https://github.com/)

*Step 2:*
Create a Profile on [Github and sign up](https://github.com/)
Fill in all the necessary fields, e.g., profile picture, name, and Bio information.

**Congratulations! You have successfully created a GitHub account.**

#### How to Install Git / Gitbash : ####

*Step 1:*

Open your browser and search for Git. OR follow this Link [Git Install](https://git-scm.com/install/windows)
 
*Step 2:*

Select the Operating system you are installing git on, i.e., Windows/ Mac os / Linux, etc

*Step 3:*

Click the hyperlink "click here to download" (as shown below)


![Git download](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/c1wgl9w3iyl4pw9n03l5.png)

*Step 4:*

Once the program has finished downloading on your machine,open and run the program.


> **Be sure to pick Visual Studio as your default code editor on git when going through the steps of installation**


***Follow each step carefully as instructed until you successfully finish installing it.***

-------------------------------------------------------------------------

### How to connect your Git to your Gitbash account using commands. ####

**Follow the following steps**

*Step 1:* Launch your git

*Step 2:*  Use the commands listed below in the following order.

- ***Command to check your git version***

`git --version`

- ***Command to configure your name and email***

`git config --global user.name "enter your name"`
`git config --global user.email "enter your email"`

>Please use the same name and email used to create your github account


- ***Command to check that your configurations are successful***

`git config --list`

- ***Command to generate an SSH key*** ( This is your unique digital identity)

`ssh-keygen -t ed25519 -C "email"`

- ***Command to make an agent for your sshkey***

`eval "$(agent-ssh -s)"`

- ***Command to add the agent.***

`ssh-add ~/.ssh/id_ed25519`

- ***Command to print or publish the agent***

` cat ~/.ssh/id_ed25519.pub`

***Now let's connect gitbash to github***

1. Follow the path provided by git to where your key is stored >> Open it using Visual Studio and copy it to your clipboard

2. Open your github account >> Go to settings >> Got to SSH & GPG keys.

3. Click add new SSH key >> Paste the key you had copied earlier in VS stduio.

***Congratulations! you successfully connected your git and GitHub accounts***

**Command to verify connection**

`ssh -T git@github.com`

*You should get a confirmation like shown below:*

![Git](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/pq3vyizvp1ry51chzchn.png)

------------------------------------------------------------------------

## **Now Let's learn a few more commands on git!** ##

### 1. Version Control on git ###

Git is the most commonly used software for version control because of the following features:

- It takes a snapshot of every commit in the entire project.

- It provides an audit trail of all changes made to the code, who made the changes, what was changed in the code, and the date and time it was changed.

- It can restore any version of the project because it keeps a permanent, unaltered record of every commit made in the entire project.

### 2. Push and Pull code on git. ###

***Pushing*** and ***pulling*** are terms used to refer to the communication between your local machine and a remote server repository where code is stored (github in this case). 

- **Pushing** - is using a specific command or an inbuilt graphical interface tool, like in [Visual Studio](https://visualstudio.microsoft.com/), to send your commits/code to a shared repository (like on GitHub) where other developers can see and interact with it. Can be referred to as *upload*

`An example of a command to push code`

```
git add
```

- **Pulling** - is using a specific command or inbuilt GUI tool to retrieve specific changes made from a remote repository and downloads and merges them into your code.

`An example of a command to pull code`

```
git pull --rebase

```
### 3. Tracking code on git. ###

Tracking code on git is monitoring any unsaved modifications and the history of any permanent changes that have been made to the project.

## Below are a few commands to track any changes in your work directory. ##

- ***To check the project's current overall status***

`git status`

- **To view exact code changes**

`git diff`


- **To check the changes waiting to be committed (staged)**

`git diff --staged`


- **To check full history or logs**
`git log`


- **For a condensed view of your history**


`git log --oneline`


- **For history of a specific file**


`git log --[filename]`


- **To show a detailed view of all your commits**

`git show  --[commit-hash]`

--------------------------------------------------------------------------

### Thank you for reading my article to the end !! ###

I hope you find it informative and educational. Please comment and let me know what you think about my article!!

Adios, until the next one.

**Signed**
**Jules.**

