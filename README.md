# GIT-Commands
## ---> GIT Revert
1.First we have to see the logs in order to get the commit ID which we want to revert
```
git log
```
This will list the commit logs with commit ID
2. Then you can copy the respective commit ID and
```
git revert {commitID}
```
This will revert the commit and goes to the previous commit state.
**Note:** It'll create one more commit like "Revert commit {ID}"

## ---> GIT Cherry Pick
We use cherry pick to get the changes from particular commit
### For instance,
If I added hello world on the first commit, I can able to get those particular change which i did in that commit
1. For that, Same first we need to list the logs
```
git log
```
2. Then copy the respective commitID the one which you want to get the changes
```
git cherry-pick {commitID}
``` 
## ---> GIT reset

The git reset command in Git is used to reset the current branch to a specific state. It is a powerful command that can be used to undo changes in various ways. There are three primary modes of git reset: soft, mixed (default), and hard.
1. **Soft Reset** (--soft):
  This mode resets the branch pointer to a specific commit, but it keeps your changes in the staging area.
```
git reset --soft <commit>
```
2. **Mixed Reset**(Default)
   This mode resets the branch pointer and the staging area to a specific commit, but it leaves your changes in the working directory as uncommitted changes.
```
git reset <commit>
```
3. **Hard Reset**(--hard):
   This mode resets the branch pointer, the staging area, and the working directory to a specific commit. It discards all changes.
```
git reset --hard <commit>
```
4. **Reset to HEAD**:
   If you want to reset to latest commit (HEAD), you can use `HEAD` as a reference
```
git reset --hard HEAD
```
5. **Reset to a Single FIle**:
   You can also reset a specific file to the state of a particular commit.
```
git checkout <commit> -- <file>
```
