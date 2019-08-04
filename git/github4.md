# [Github项目合作开发流程](https://www.cnblogs.com/schaepher/p/4933873.html)
## *0.前期准备
项目负责人新建一个项目，更改队友的权限，必须审核后才可以push到团队项目
## *1.创建开发项目
项目负责人创建分支，一般默认的master分支用来发布稳定版本，示例采用dev分支作为操作分支
## 2.fork项目到个人仓库
队友将团队项目fork到自己个人仓库
## 3.Clone项目到本地
将对应的**个人仓库**clone到本地
1. `git clone ssh-url`后本地会多一个名为项目名称的文件夹。ssh-url的获取及设置查看[此处](https://www.cnblogs.com/schaepher/p/5561193.html#local)
2. `git branch`-查看本地分支,`git branch -a`-查看本地与远程remote所有分支**注意：如果上述两个命令无反应，记得文件要切换到新下载的文件夹下**
3. `git checkout -b dev origin/dev`的意思是，创建一个本地dev分支(-b)，并把远程的dev分支(origin/dev)的内容放在该分支内，接着切换到该分支（checkout）
4. `git branch`-查看本地分支,`git branch -a`-查看本地与远程remote所有分支进行检验
5. `git checkout master`可以切换回master分支，上面完成后就可以在**本地进行开发**了
## 4.和团队项目保持同步
1. `git remote -v`查看有没有设置upstream
2. `git remote upstream 团队项目地址`添加upstream远程
3. `git remote -v`查看upstream是否设置成功
4. `git fetch upstream`获取团队项目的最新版本
5. `git merge upstram/dev`将源分支（upstream/dev）合并到**当前分支(你在本地的开发分支)**
## 5.push修改到自己的项目上
`git push`将本地的修改同步到自己的GitHub仓库上（在本地dev分支下push）
## 6.请求合并到团队项目上
登陆自己的github中，进入fork的仓库，点击**pull request**
在最新界面中，左侧表示收件人信息，右侧表示发件人信息，确认信息后，右下角Create pull request即可
## *7.团队项目负责人审核以及后续
团队负责人进行审核、合并等后续工作


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
