# 远程仓库的配置与使用（remote）
## 添加远程仓库
`git remote add [name] [url]`
示例：`git remote add practice https://github.com/pzq-pzq/practice.git`
说明：上述中的name与erl一一匹配，将name作为连接的标识

## 删除、修改远程仓库
修改可采用先删除后添加
删除远程仓库`git remote rm [name]`
示例：`git remote rm practice`

## 查看远程仓库列表
`git remote -v`

## 推送到特定的远程仓库
`git push [remote] [branch]`
示例：`git push practice [暂空]`
说明：这样每次输入不同的remote,便可上传到不同的远程仓库

## 获取远程仓库的内容
`git pull [remote] [branch]`
示例：`git pull practice [暂空]` 
说明：获取name为practice的远程仓库的内容

## 分支的操作
### 列出分支
`git branch`

## 结语
以上仅整理了部分常用的git命令，具体清单可以可以查询[Git命令清单](http://www.codeceo.com/article/git-command-list.html)

学习、成长是一辈子的事

2019.8.1于哈工大
