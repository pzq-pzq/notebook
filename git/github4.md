`git push pzq-git `
`git merge [name]`将名称为[name]的分支与当前分支合并

# [git拉取远程分支到本地](https://cnblogs.com/sandea/p/9855062.html)
## 1.查看远程分支
`git branch -r`
## 2.查看本地分支
`git branch`
## 3.拉取远程分支
`git checkout -b 本地分支 origin/远程分支`
## 4.拉取远程分支
`git pull origin 远程分支`
## 5.建立分支
`git branch --set-upstream-to origin/远程分支名  本地分支名`
## 6.拉取分支
`git pull`
## 7.遇到本地冲突，先删除本地分支，再重新拉取远程分支
`git branch -D 本地分支名称`

# [新建远程分支](https://www.cnblogs.com/dyh-air/articles/8931373.html)
`git push origin bendi:bendi`
将本地分支和remote的分支绑定，以后直接在本地分支下，git pull与git push即可
