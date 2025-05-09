# To check

- git -v 

- git config --system --list

- git config --global --list

- git config --list 

# To set 

- git config --global user.name "Input_username"
- git config --global user.email "Input_email"

# Basic command

- git status

- git init

- git add, git add .

- git commit -m "Your_Message"

- git log // lists the commits details in local

- git show COMMIT_ID // shows the changes.

- git remote add origin URL // to connect your local repo to the remote repo using URL.

- git clone Url // to clone the repo from remote to local.

# git pull and push

- git pull 

- git push 

# git ignore

- create a file called = .gitignore

- below are to ignore files in different ways.
--> a) for specific file = sample.txt
--> b) for root path folders only = /temp
--> c) for root path folders and anywhere in repo = temp/
--> d) for specific file formate = *.txt

# git previous version

- git log --oneline // to get the oneline commit id details.

- git checkout Commit_ID // to go to the previous or any level of commit id in local repo.

- git revert 
=> it is used to undo changes introduced by a specific commit while preserving the commit history

Example
- git revert Commit_Id
- git revert HEAD
- git revert HEAD~number
- git revert Commit_ID --no-edit  // imp
- git revert Commit_ID1 Commit_ID2 ....   // can revert multiple commits in one shot.

- git reset
=> it is used to move the HEAD pointer to a specific commit, it modifies the commit history by adjusting the HEAD pointer.

Eaxmple
- git reset commit id // 
- git rest HEAD~number
- git reset --soft commit id // comes to stagging area
- git reset --hard commit id // all history commits are deleted


- revert vs reset
-> revert // used for remote repo commits
-> reset // used for local repo commits 

# git branches

- git branch     // list branches

- git branch Branch_Name       // create the branch

- git checkout -b Branch_Name  // if not exists creates and switch branch

- git merge Branch_Name  // merge branch

- git branch -d Branch_Name  // delete branch

# git merge conflicts

- if two branches modify the same lines of code in a file.
- if one branch renames or moves a file while another branch modifies it.
- if a file is deleted in one branch and modified in another branch.


# git rebase

- to change the base branch to the latest one for the child/feature branch.
- make sure to be in child branch to perform the command.

- example = git rebase master