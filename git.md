# git commands for General Use
## git Clone
- git clone <uri>
- git checkout -b <new branch name>
- git push --set-upstream origin <new branch>
- git checkout <branch name>

## Git Merge from master to current branch:

- git checkout my_branch    # move on your branch (make sure it exists)
- git fetch origin          # fetch all changes
- git pull origin master    # pull changes from the origin remote, master branch and merge them into my_branch
- git push origin my_branch # push my_branch

## To abort the merge:
- git merge --abort


## git stash:

- git stash       # to stash your changes,
- git stash -u    # to stash untracked changes
- git stash -a    # to stash all untracked and ignored changes,
- git stash list  # to list all the stashes
- git stash save "remove semi-colon from schema"      # to name the stash on specific name.
- git stash pop stash@{1}   Or  git stash apply stash@{1} 
- git stash clear     # to remove all the stashes
- git stash drop <Stash_id>       # to remove the particular stash from the stash list.
 
- git stash show stash@{0} --patch
- diff --git a/console/console-init/ui/package.json b/console/console-init/ui/package.json
 
- git stash branch test_2 stash@{0}   # to save stashed changes to new branch and to move to that branch.
- git stash create "simple stash"     # to create the new stash from command without pushing it to the reflog.
- git stash store -m "simple stash testing..."    # to push stash entry to stash reflog.



## git commit:
- git commit -m "Here is the commit message"
    - Comment
- git push
- git pull
- git add .
- git add file,names,list
- git reset
- git add *.java
- git reset *.java
- git reset file,name,list

