# Git


### Reset last Git commit
```
git reset --hard HEAD~1
```



### Merge one branch into another
Example you want to merge (bring the changes from) UAT changes to Develop, you must executhe the merge command inside the target branch.
```
git merge uat
```



### How to make a commit with a message
```
git commit -m  "Merge UAT to Develop"
```



### How to amend a commit.
If you have a commit (better if you have not push it yet) and you want to append it some other changes you can do this with an amend.
```
git commit --amend -m "TicketIDHere"
```
