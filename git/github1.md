# 1.使用github（目的、基本概念、注册账号）
## 目的
托管代码
## 基本概念
- 仓库（Repository）
>用来存放项目代码，每个项目对应一个仓库
- 收藏（Star）
>收藏项目，方便下次查看
- 复制克隆项目（Fork)
>fork的项目是**独立存在**的，这里修改不会影响复制的源文件
- 发起请求(Pull Request)
>将自己的文件向对方Pull Request(简称PR)申请，经过对方review同意后，可以将文件接收并合并
- 关注（Watch)
>关注项目，当项目更新时可以接收到通知
- 实务卡片（Issue）
>发现bug，但目前没有成型的代码，需要讨论时候使用
- Github主页
>github官网，用户的动态等信息
- 仓库主页
>项目的基本信息
- 个人主页
>个人的基本信息，类似于社交的，关注的人等信息
## 注册GitHub账号
[github官网](https://github.com/)按照提示输入信息，留下邮箱和用户名等信息，一般设置选择为非私有的项目，即公开的项目。相对简单，不在赘述。
- fanqiang助手，在github中搜索**shadowsocks**

# 2.使用Github(创建仓库、仓库主页说明)
首先**验证邮箱**后，便可以创建仓库等工作（验证邮箱时若收不到邮件，注意邮箱垃圾，或者添加白名单）
## 个人主页
个人主页-Repositories-New
>输入Repository name-->项目名称（英文）
>勾选Initialize this repository with a README（仓库中会多一个readme.md文件）
## 仓库主页
>`Create new file`    -->创建文件
>`Upload file`        -->上传文件
>`Find file`          -->搜索仓库文件
>`Clone or download`  -->搜索仓库文件

# 3.使用Github(仓库管理)
## 新建仓库文件
在仓库主页下，点击**Create new file**
>仓库名/仓库下文件名
>最下方，Commit new file-->输入备注信息
## 仓库文件的操作
>在仓库主页下，点击文件名，到文件详情页点击右侧的笔logo,可以做删除和修改动作
>在项目文件主页下，修改后也要进行描述，最下方，Commit new file-->输入备注信息
>在仓库主页下，点击描述，可以查看该文件提交详细信息
>在仓库主页下，点击**commits**显示历史记录（作用同上）
## 删除文件
>在仓库主页下，点击文件名，点击最右侧删除，
>>在项目文件主页下，删除后也要进行描述，最下方，Commit new file-->输入备注信息
>在仓库主页下，点击**commits**显示历史记录，可以显示删除操作记录
## 上传文件（Upload files）
>在仓库主页下，点击Upload files可以直接上传文件，路径选择或者拖拽操作
## 搜索文件（Find files）
>在仓库主页下,点击Find files后，输入文件名，即可搜索
>>在仓库主页下,键盘输入**T**可以直接切换到上述页面
## 下载文件（Clone or download）

# 4.使用Github(Github Issues)
## 访问别人的github仓库主页
>点击Issues，输入自己反馈的信息，在write中填写，在preview中预览
## 登陆自己的github
>点击Issues，就可以看到别人提交的信息，在write中填写**回复**，在preview中预览，Close issue

# 5.使用Github(基本概念实战操作)
## fork项目
## 发起更新请求(Pull Request)
>在仓库主页下，点击**New pull request**
## 开源项目流程
>1. fork项目
>2. 修改自己仓库的项目代码
>3. 新建 pull request
>4. 等待作者操作（合并审核）

# 6.安装Git
## 下载与安装Git
[下载地址](https://git-scm.com/downloads)，下载完毕，windows系统按照提示一步步点即可。
## 检验是否安装成功
桌面鼠标右击，出现两个Git菜单，即安装成功

# 7.Git基本工作流程
## Git三种区域
- 工作区（Working Directory）
>添加、编辑、修改文件等动作
- 暂存区
>暂存已经修改的文件最后统一提交到git仓库中
- Git仓库（Git Repository)
>最终确定的文件保存到仓库，成为一个新的版本，并且对其他人可见
## 向仓库中添加文件流程
工作区-->暂存区-->Git Repository(Git 仓库)
`git status`-->查看当前文件状态
`git add name.py`-->将文件从工作区传到暂存区
`git commit -m '提交描述'`-->将文件从暂存区上传到Git 仓库
![向仓库中添加文件流程图]()

# 8.Git初始化及仓库创建和操作
## 基本信息设置
1. 新建一个工作目录，空白处右击**Git Bash Here**
2. 设置用户名
`git config --global user.name 'user-name'`
3. 设置用户邮箱
`git config --global user.email '123456789@qq.com'`
4. 查看设置
`git config --list`
5. 说明
1中user-name为自己的github账户名称,唯一的
2中最后的引号中为邮箱名称，名称加后缀
该设置在github仓库主页显示了谁提交了该文件
## 初始化一个新的Git仓库
1. 上述文件夹下，新建test夹（mkdir wenjian）
2. 在文件内初始化git(创建git仓库)
`cd test`更改工作路径，或者鼠标点击也可
`git init`生成一个.git隐藏文件，若不显示，设置显示隐藏文件
## 向仓库中添加文件流程
1.  在test文件夹中新建一个文件a1.py
2. `git status`查看当前文件状态
3. `git add a1.py`将文件从工作区传到暂存区
4. `git status`查看当前文件状态
5. `git commit -m 'add a1.py'`将文件从暂存区上传到Git 仓库
6. `git status`查看当前文件状态
## 修改仓库文件
1. 打开a1.py文件，修改文件（`vi a1.py`）
2. `git status`查看当前文件状态
3. `git add a1.py`将文件从工作区传到暂存区
4. `git status`查看当前文件状态
5. `git commit -m 'add a1.py'`将文件从暂存区上传到Git 仓库
6. `git status`查看当前文件状态
## 删除仓库文件
1. 删除文件（`rm -rf a1.py`)
2. `git rm a1.py`
3. `git commit -m '删除仓库文件'`

# 9.Git管理远程仓库
## 使用远程仓库的目的
备份，实现代码共享集中化管理
## Git克隆操作
>工作区-->暂存区-->Git Repository(Git 仓库)-->远程仓库(`git push`)
- 目的
>将远程仓库（github）对应的项目复制到本地
- 代码
`git clone 仓库地址`
>仓库地址在仓库主页右侧**Clone or download**处复制得到
## 具体操作
1. 删除本地的test文件夹，避免冲突
2. 右击**Git Bash Here**,输入`git config --list`查看信息
3. `git clone 仓库地址`出现：Clone into 'test'，将远程仓库的文件复制到本地
4. ** `vi a1.py`文件操作,`wq`保存**
5. **`git add a1.py`**
6. **`git commit -m '第二次提交'`-->将文件从暂存区上传到**本地Git 仓库****
7. `git status`-->查看当前文件状态
8. **`git push`上传到**远程Git 仓库****
## 常见错误
The request URL returned error:403 Forbidden while accessing 
>私有项目，没有权限，输入用户名密码，或者远程地址采用这种类型
`vi .git/config`
```
将[remote "origin"]
    url = https://github.com/用户名/仓库名.git
修改为：
将[remote "origin"]
    url = https://用户名：密码@github.com/用户名/仓库名.git
```

# 10.Github Pages 搭建网站
## 个人站点
### 访问
`http://用户名.github.io`
### 搭建步骤
1. 创建个人站点-->新建仓库（注：仓库名必须是‘**用户名.github.io**’）
2. 在仓库下新建index.html文件,作为网站首页
## Project 项目站点
### 访问
`http://用户名.github.io/仓库名`
### 搭建步骤
1. 进入项目主页，点击settings
2. 在settings页面，点击**Launch automatic page generator**来自动生成主题页面
3. 输入基本信息（项目名称、目描述、具体内容），最后右下角确认
4. 点击设计主题页面，不同的UI
5. 右上角确认，生成网页







