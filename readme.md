### GIT COMMANDS
 

## ADD,COMMIT,PUSH
 
```
Git add -a or git add -A -> to add all updated ,deleted, updated files
```

 

```
Git add -a . -> it will only add new files and updated files.

 
```
Git add -u -> looks at all the already tracked files and stages the changes to those files if they are different or if they have been removed.
```
 
```
Git add filename -> to add that file
```
 
```
Git commit -m “my commit message” => to commit files
```
 
```
Git status -> to check files status
```
 
```
Git commit -am 'message' -> add and commit together
```

## CHECKING FILES & COMMITS
 
```
Git ls-files -> check which files are being tracked
```
 
```
Git reset HEAD filename -> file will come back to unstaging env
```
 
```
Git checkout --filename -> to stash changes of a particular file
```

```
Git help log -> To check options
```
 
```
Git log -> To check history of files
```
 
```
Git log --oneline --graph --decorate -> to get commit in one line and in a proper way
```
 
```
Git log commit id...commit id -> it will return all the commits b/w these ids
```
```
Git log --since=”3 days ago” -> give commits of last 3 days
```
 
```
Git show commitid -> to check changes of specific commit
```
 
```
Git config --global alias.variablename “command to be issued” -> to create your own commands
```


COMPARISON COMMANDS
 
```
Git diff -> to check what’s changed in the files local vs staged.
```
 
```
Git diff HEAD -> to check what’s changed in the files local vs repo
```
 
```
Git diff --staged HEAD -> to check what’s changed in staged vs repo
```
 
```
Git diff -- path of file -> to check diff of a specific file
```
 
```
Git diff commitId HEAD -> to check diff b/w commit with HEAD
```
 
```
Git diff HEAD HEAD^ -> diff b/w head and head minus 1 commit
```
```
Git diff startCommitId endCommitId -> startCommitId to check diff b/w two commits
```
 
```
Git diff master origin/master => diff b/w what is committed vs origin master
```
 

BRANCH AND MERGING
 
```
Git branch -> to check your current branch
```
 
```
Git branch -a -> return list of branches
```
 
```
Git branch branchName -> to create a new branch
```
 
```
Git checkout branchName -> to shift on another branch
```
 
```
Git checkout -b branchName -> create and shift to branch
```
 
```
Git branch -m branchName newBranchName -> first go to master and run to change the branch name
```
 
```
Git branch -d branchName -> first go to master and run To remove a branch
```
 
```
Git merge branchName -> first go to master and run to merge a branch in it.
```
```
Git merge branchName --no-ff -> first go to master and run to merge a branch in it.
```
 
```
Git rebase branchName -> this will add changes of branchName in current branch
```
 
```
Git rebase --abort -> to abort changes of rebase
```
 

STASHING
 
```
Git stash -> to remove and stash your current changes (only tracked files).
```
```
Git stash apply -> to get back the code that you have stashed
```
 
```
Git stash list -> to see all the stash that you have done earlier
```
 
```
Git reset --hard HEAD -> resetting your code back to HEAD
```
 
```
Git stash drop -> to remove the stash you have done
```

```
Git stash -u -> to stash all files including untracked files
```
 
```
Git stash pop -> it will apply stash changes and also going to drop the stash
```
 
```
Git stash branch branchName -> if you want to apply stash changes to another branch
```
 
```
Git stash save “message” -> to save stash with a message
```
 
```
Git stash show @{index}-> to see what is in stash
```
 
```
Git stash apply @{index}=> to apply specific stash
```
 
```
Git stash clear -> to drop all stash at once
```


TAGGING
 
```
Git tag tagName -> create a tag (lightweight tag) on a commit
```
 
```
Git tag --list -> to check all the tags
```
 
```
Git tag --delete tagName -> to delete a tag
```
 
```
Git show tagname => to check tag details
```
```
Git tag -a tagName -m “message of tag” -> to create a annotate tag
```
 
```
Git diff tagNameA tagnameB -> diff b/w both tags
```

```
Git tag -a tagName commitId -m “message of tag” -> to apply the tag with old commit
```
 
```
Git tag -a -m “message” tagName -f correctCommitId -> to update a tag from one commit to another
```
 
```
Git push origin tagName -> this will push changes of commit along with tag
```
 
```
Git push origin master --tags -> push master branch along with all the tags
```
 
```
Git push origin :tagName -> to delete a tag from pushed master
```
