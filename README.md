# GitHub Tutorial

_by Mei Ting Ieong_

---
## Git vs. GitHub  
#### What is Git?  
* Git is a version control that keeps "Snapshots" of code.  
 * Version control is like a timeline that you can see the changes you havemade in the past.  


#### What is GitHub?
* GitHub is in the cloud (internet) where you can store your code.  
* GitHub visually keeps track of changes by refering back to the commit.
* People can collaborate on someone else's project very easily.

#### What is the difference between Git and Github?  
* Git does not require github but github does require git.  




---
## Initial Setup (one-time setup)
1. Sign up for for an account in [Github](github).  
2. Create an username and password then click free account.  
3. For the SSH key or HTTPS, go to github and click the profile icon in the top right corner.  
4. Click settings and add the key you want (SSH or HTTPS).  
5. Switch to your IDE and find the SSH/HTTPS and copy/paste it into GitHub. Click add key.  
6. In IDE, type `ssh -T git@github.com` or `https -T git@github.com` then type yes.  
7. Type `git config --global user.name "your_name"`.
8. Type `git config --global user.email your_email`.
9. You're done now and you will not have to do this unless you create a new repo.

####_Please read this!!!!_  
* HTTPS stands for Hypertext Transfer Protocol Secure and if you are using this, you would have to sign up for your username and email everytime you login. 
*  SSH stands for Secure Socket Layer and if you're using SSH, then you will only ask to sign in once and the computer will remember you as long as you're using the same repo.  
*  The `git config --global user.name` and email are important because that is how you get the credit for wrting the code.    


---
## Repository Setup
* In order to use git in your IDE, you have to type `git init`. 
 * By doing so, you're telling the IDE that you want to turn on git and start making commits.

**Here are the steps to create a new repository.**  
1. Go to IDE, type `mkdir first-repository`.  
2. Type `cd first-repository` to go inside the repo.  
3. `git init`  
4. `git config --global user.name "your_name"`  
5. `git config --global user.email "your_email"`  
** Now, we need to create a new file called README.md**  
1. `touch README.md`  
2. open README.md and type in something like "This is my first repo"  
3. save it and add it to the stage by type in `git add README.md`  
4. commit it by `git commit -m "add README.md"`  
**We need to create a remote in order to push the code to Github**  
1. go to github > top right > click the + sign > select new repository.  
2. The name for the repo needs to match the name in the IDE. So in this case. we would name it "first-repository".  
3. Click create repository.  
4. On the top of the new page, they would ask you to choose SSH or HTTPS, so pick the one you like.  
5. There will be two boxes of code, look at the second box "push an existing repository to the command line" and copy/ paste the code to your IDE _LINE BY LINE_.  
5. refresh the github page and you should see the changes that you made.  

_You use `touch` for word documents_  
_Commit often so you can look back at the changes you made!!!_
 
---
## Workflow & Commands  
**Workflow of Commands**  

* git init  
_edit file(s)_
* git status→ you can see which file that have been edited and it should be red   
* git add file.ext  
* git status→ you now can see which file have been added to the stage and it should be green now.  
* git commit -m "some message"→ write a short and specific message in present tense  
_repeat_  

**Push**  

* In IDE, type `git remote add origin URL`  
* remote→setup a connection between our local repo and the external repo in github  
* add→ adding the remote repository   
* origin→ origin is just a nickname for the repo and origin is the standard one  
* URL→ the location of the remote repo(can be SSH or HTTPS)  
* Type `git push -u origin master`   
* push→ sending commits from local repo to remote repo(github)  
* -u→ stands for "upstream" and it remembers which remote repo you want to push so you don't have to write the entire code again in the future  
* origin→ the remote you're pushing to  
* URL- the main branch of the project  
 **This is a one-step setup so you just need to type `git push` in the future as long as you're using the same local repo**

**Clone**  
By cloning the file, you're making a copy of your code from the remote repo to your local repo.  

* Go to github and open your repo  
* Go to the right sidebar and copy the URL  
* In IDE, type `git clone URL` and you will find that your repo is back.  

**Forking**  
Forking is different from cloning because forking is making a copy of someone else's repository to your remote repository and then to your local repo. However, you're only making a copy of your remote repo to your local repo for cloning. Therefore, you cannot make any changes on someone else's project with cloning.

* Go to the repository of the person that you want to fork and click the fork botton  
* Now you just see your name on the URL so copy the URL  
* Type `git clone URL`   


 _what happen if you want to make suggestion to that person?_  





