### How to set your username so github does not ask you again (HTTPS way)
* Instead of using
```
 git remote add origin https://github.com/Joshua-Lopest/gittips.git
```
* use it while adding "your_username@" before github.com
```
 git remote add origin https://Joshua-Lopest@github.com/Joshua-Lopest/gittips.git
```
### Quickly override unwanted commits
* ATENTION: Keep in mind this proccess IS GOING to forcefully revert to a previous commit. Any other commits after this is going to be lost. Use with caution.
* You need to revert to a previous branch. You can do it by using the commit's SHA code
```
git reset --hard 676fd4cc273f6c9035278e6292321f606dd63ddc
```
* or by expliciting how many commits you want to go back
```
git reset --hard HEAD~[number of commits]
```
* then, force a push, so remote master is going to be updated
```
git push --force origin master
```
### Quickly commit adding all tracked filles
* Simply state a -a within the commit, so you add all tracked files, without need of using git add.
```
git commit -a -m "commit message"
```
