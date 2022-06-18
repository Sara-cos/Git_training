# Git_training
Perform the git commands on available tutorials (Microsoft Learn Student Ambassadors)

What is **local repository** and **remote repository**?
Local repositories reside on the computers of team members. In contrast, remote repositories are hosted on a server that is accessible for all team members - most likely on the internet or on a local network.

**HEAD** is the reference to the most recent commit in the current branch. This means HEAD is just like a pointer that keeps track of the latest commit in your current branch.

**Git history** is nonlinear: a directed acyclic graph (DAG) or tree. 

**Stashing** : Often, when you’ve been working on part of your project, things are in a messy state and you want to switch branches for a bit to work on something else. The problem is, you don’t want to do a commit of half-done work just so you can get back to this point later. The answer to this issue is the git stash command.

**Staged** files are files that are ready to be committed to the repository you are working on.

**gitignore** or Git Ignore : files or parts of your project, you do not want to share. Git can specify which files or parts of your project should be ignored by Git using a .gitignore file. Git will not track files and folders specified in .gitignore. However, the .gitignore file itself IS tracked by Git.


#### To see the status of your files
```
git status
```

#### Git version
```
git --version
```

#### Changing the branch or Chcekout the branch
```
git checkout existing_branch
```
```
git checkout -b new_branch
```

#### Check all the branch
```
git branch -a
```

#### Staging 
All new and updated files are staged

```
git add --all
```
```
git add -A
```
```
git add .
```

#### Stashing
Saving the work before leaving the branch/ switching the branch. *If you don't want the current changes to be commited*
```
git stash
```
```
git stash push
```
To check the history of stashings

```
$ git stash list
stash@{0}: WIP on master: 049d078 Create index file
stash@{1}: WIP on master: c264051 Revert "Add file_size"
stash@{2}: WIP on master: 21d80a5 Add number to log
```
To switch/apply the stash
If recent/current stash
```
git stash apply
```
If any specific previous stash, *Here it takes to stash 2/two stash before*
```
git stash apply stash@{2} 
```


#### A list of remote repositories and their URLs
```
git remote -v
```


#### Cherry picked
commit is being cherry picked as the new HEAD of the commit history
```
git cherry-pick commit_name
```

#### Reseting previous commit
```
git reset hard HEAD~5
```
The current branch’s HEAD is reset the current branch to the commit just before the last 5 (see man gitrevisions for details about this notation and other cool alternatives like HEAD@{2 days ago}). As it is a hard reset, it will also overwrite every change in the working tree as well. 


#### Merge the previous set of commits
```
git merge --squash HEAD@{1}
```
prior commits are squashed into a single commit.

#### Merge a branch to another branch

Chcekout to the branch (where you want it to be merged) and then merge it
```
git merge branchname
```


#### How to get help for perticular command
```
git (command) -help
```

#### For connecting the local repository to remote repository, 
```
git remote add origin
```
```
git remote add new
```
