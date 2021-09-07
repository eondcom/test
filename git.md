git init
git add git.txt
git commit -m "first commit"
git config --global user.email "eond@eond.com"
git config --global user.name "eondcom"
git push
```
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using      

    git remote add <name> <url>

and then push using the remote name

    git push <name>
```    
git remote add test https://github.com/eondcom/test.git

```
…or create a new repository on the command line
echo "# test" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/eondcom/test.git
git push -u origin main
…or push an existing repository from the command line
git remote add origin https://github.com/eondcom/test.git
git branch -M main
git push -u origin main
…or import code from another repository
You can initialize this repository with code from a Subversion, Mercurial, or TFS project.


```

To push the current branch and set the remote as upstream, use
```
    git push --set-upstream test master
```
딱 한번만 페어링 해주면 된다.
로컬저장소와 원격저장소 브랜치 이름이 달라서..

정리
git init
git add git.txt
git commit -m "first commit"
git config --global user.email "eond@eond.com"
git config --global user.name "eondcom"
git remote add test https://github.com/eondcom/test.git
git push --set-upstream test master
git pull