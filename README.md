
# Git




#### Install git by offical website

 - Setup user name and password globally  so other developer know who has commited the code

 
Set by config method


```bash
~ git config --global user.name = "your name here"
~ git config --global user.email= "your email here"
```

Set by edit method

```bash
~ git config --global edit
~ git config --global user.email/user.name (for check current email and name)

```

### Commands


```bash

~git int  ( initial repo create for track changes )
~git status  (check the files chnages in local and compare the reomote branch code)
~git add .  ( track file and add in stating area )
~git commit -m "message of commit"   ( commit the changes )
~git log   ( check the commit logs )
~git checkout "has code of commit"   (swtich between commits)
~git checkout master  (swtich in main commit )
~git branch ( show all branches )
~git branch branch_name  (create new branch)
~git checkout  branch_name  (switch between branch)
~git checkout  -b  branch_name  (create new  branch and switch that branch)
~git merge branch_name  (merge branch into current branch)
~git push (push commit to the branch)


```

### Create git repo on github

---------------------Do Folow this steps one time setup----------------------

```bash
~git remote add origin remote_repo_url  (connect remote branch to local so we can sync)
~git remote -v  (check remote origin for fetch and push
~git branch -M master ( command is used to rename a branch in Git.)
~git push -u origin master (push the branch to the origin)
```


----------------------------------------------------------------------------


### Add collaborators 

github -> repo -> setting -> manage access invite collaborators by using Email 📧 



### Opern source Contribution

git repo -> click on fork  (this will create same clone repo on your github account )

```bash
~git clone git_repo_url_that_you_want_to_clone_on _your_local_machine
~git add . 
~git commit -m "message" 
~git push
```

- Above  steps push your code to your remote branch
- Our branch is ahead of original  code of forked branch

- so now we have to create pull request from github

- git-repo -> contribute button -> click create pull request -> click create pull request -> add message and click on create pull request


- Now Original source repo author can approve and commit that changes on respected branch 

- git repo -> click on pull request -> click on pull request  that you want to check-> file changes and check the chances -> click on review changes ->  add message and approve the changes -> now you can merge the pull request  by click on merge pull request  button



### git fetch vs git pull

- git pull = git fetch + git merge

- git fetch only pull the lastest chnages on local branch not merge on local branches  so you can review  and merge as per you need
- git pull fratch the chnages on local branch and also merge that at a same time so you can not review  the code before  conflict raise 


### Git stash

- git stash is used when you want to save you uncommit changes save in memory and and revert  as last commit then add you argent  changes  and then after you want to continue on that stashed uncommited changes

- example. 
 you are working on some features and your manager  want some urgent  changes
so you can stash that changes  so you code reverts  as previous  commit and make that urgent  changes and push the code
after completed the urgent  task you can continue  on your stashed  code by apply  it

```bash
~git stash save "name of stash"   (add your current changes in stash memory)
~git stash list  (show list of stashed changes with unique id)
~git stash apply  {unique id from list command } (apply stash on current workings branch)
~git stash drop  {unique id from list command } (delete particular stash)
~git stash pop  
~git stash clean (remove all stash from memory)
```
