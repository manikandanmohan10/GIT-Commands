# GIT-Commands
## GIT Revert
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
