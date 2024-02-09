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

## GIT Cherry Pick
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
