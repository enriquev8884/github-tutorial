# GitHub Tutorial

_by Enrique Vivar_

---
## Git vs. GitHub
###Git: _Version control: Keeps "snapshots" of code_
* Does not require Github
* Used to :  
 * edit files
 * add files
 * commit them  

###Github:
* stores code in a cloud _(github.com)_
* able to tracks changes
* easily collaborate on files
* requires git 
* runs in the command line

---
## Initial Setup  
####Once a github account is created, you would have to connect your account _[cloud]_, to your terminal _[C9]_  
1. Create a c9 account  
2. Go to settings and click on SSH Keys  
3. Copy the SSH Key  
4. Head over to your Github.com account   
5. Go to settings  
6. Click on tab named SSH Keys  
7. Click on add SSH Keys    
8. Add a title, paste the SSH Key 
9. Save!

####Once saved, you'll also need an identity for your work. With `git config` you will need to create a username and add an e-mail.
  

`git config --global user.name`  
#####_user.name being desired name_
`git config --global user.email` 
#####_user.email is e-mail_

####With that you set your identity up, you're all good to go
---
## Repository Setup

####To start off, you will need to create a directory;
   `mkdir directory.name`   
#####_directory.name being what you want_
  
####With your new directory you will have to `cd` into it; 
   `cd directory.name`

####Within the directory, its recommended to create a README.md file;
   `touch README.md`

####Once the README.md is made, we can initialize it;
   `git init`
   
####Now that we have a repository, head to github.com and sign in.

![pic](github-repo.png)

1. Copy SSH Key and head back c9
2. Type `git remote add origin SSH Key` (SSH Key being the one you copied)
3. Then enter `git push -u origin master`
4. Now you're ready to work

---
## Workflow & Commands

*  <span style="color:red;"> `mkdir directory.name` </span> <span style="color:grey;"> creates directory </span>
*  <span style="color:red;"> `cd` </span> <span style="color:grey;"> used to go in or out of repositories </span>
*  <span style="color:red;"> `git init` </span> <span style="color:grey;"> makes directory into a repository </span>
*  <span style="color:red;"> `git help` </span> <span style="color:grey;"> used to explain commands </span>
*  <span style="color:red;"> `git status` </span> <span style="color:grey;"> to see what files are ready to be commited </span>
*  <span style="color:red;"> `git diff` </span> <span style="color:grey;"> see difference between current code and previous commit </span>
*  <span style="color:red;"> `git add` </span> <span style="color:grey;"> adds new or changed files </span>
*  <span style="color:red;"> `git commit -m` </span> <span style="color:grey;"> prepares files to get pushed </span>
*  <span style="color:red;"> `git push` </span> <span style="color:grey;"> sends commits to remote repo </span>
*  <span style="color:red;"> `git pull` </span> <span style="color:grey;"> any changes on remote repo are brought down </span>
