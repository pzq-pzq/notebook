# 新建本地git与远程remote教程
1. 在本地新建一个文件夹
>实例：新建test文件夹
2. *设置用户信息(**一次设置，全局有效，之前如果设置过，此步骤可以省略**)
- 设置用户名：`git config --global user.name 'uesr-name' `
>实例：`git config --global user.name 'pzq-pzq' `
- 设置用户邮箱：`git config --global user.email 'uesr-email' `
>实例：`git config --global user.email '1234567890@qq.com' `
- 查看设置：`git config --list`
>运行后,出现列表，显示上述设置的user-name和user-email表示设置成功
3. test文件夹内，右击**Git Bash Here**，输入`git init`
运行后会在当前文件下生成一个.git隐藏文件，如果不显示，自行百度隐藏文件设置
4. 输入`git remote add url-name url`
>示例：`git remote add work https://github.com/pzq-pzq/notebook.git`
>说明：url-name为remote的名称，后面连接为绑定的远程仓库remote的链接，具体获取方式见下图
5. 输入`git remote -v`
显示刚刚设置的url-name以及链接表示绑定成功
6. 输入`git push`即可上传，`git pull`即可将远程remote复制到本地工作文件夹
7. *如果提示失败，先输入`git pull --rebase url-name master`，后输入`git push -u url-name master`即可成功上传，并且以后仅需输入`git push`即可，只有在首次设置时设计到此步骤

# 结语

学习、成长是一辈子的事

2019.8.2于哈工大