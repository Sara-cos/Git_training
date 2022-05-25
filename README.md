# Git_training
Perform the git commands on available tutorials (Microsoft Learn Student Ambassadors)

#### git version
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
#### A list of remote repositories and their URLs

```
A list of remote repositories and their URLs
```
#### cherry picked
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


#### For connecting the local repository to remote repository, 
```
git remote add origin
```
```
git remote add new
```
