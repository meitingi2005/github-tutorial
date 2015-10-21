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


 
 
---
## Workflow & Commands