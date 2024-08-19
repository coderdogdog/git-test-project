### 基础命令



| 代码                                    | 指令             |
| --------------------------------------- | ---------------- |
| git --version                           | 版本信息         |
| git config --global user.name 用户名    | 设置用户签名     |
| git config --global user.email 用户邮箱 | 设置邮箱         |
| git init                                | 初始化本地库     |
| git status                              | 查看本地库状态   |
| git add hello.txt                       | 加入缓存区       |
| git rm --cached hello.txt               | 从缓存区删掉     |
| git commit -m "备注信息" hello.txt      | 提交本地库       |
| git reflog                              | 查看精简版本信息 |
| git log                                 | 查看详细版本信息 |
| git reset --hard 版本号                 | **版本穿越**     |
|                                         |                  |





| Linux代码           | 指令               |
| ------------------- | ------------------ |
| Ctrl + L            | 清屏               |
| ls                  | 列出当前目录       |
| ll                  | 显示目录下的文件   |
| vim hello.txt       | 生成文件           |
| yy                  | 复制               |
| P                   | 粘贴               |
| Esc                 | 退出编辑，回到命令 |
| :wq                 | 保存               |
| cat hello.txt       | 查看文件内容       |
| tail -n 1 hello.txt | 查看末尾最后一行   |
| I                   | 进入txt文件修改    |
|                     |                    |



### git分支操作

| 代码                | 指令                       |
| ------------------- | -------------------------- |
| git branch 分支名   | 创建分支                   |
| git branch -v       | 查看分支                   |
| git checkout 分支名 | 切换分支                   |
| git merge 分支名    | 把指定分支合并到当前分支上 |
|                     |                            |
|                     |                            |



### 创建远程库

- `git remote -v` 查看当前所有远程库地址别名
- `git remote add 别名 github地址`      别名就是对地址起的别名，项目名 



### 本地推送远程库

`git push 别名 本地分支`

### 拉取远程库

`git pull 别名 远程分支` 

### 克隆远程库

使用别人的代码库

`git clone 仓库地址`

不需要登陆账号

公共库

克隆：

1. 拉取代码
2. 初始化本地库
3. 创建别名



### 生成.ssh密钥目录

`ssh-keygen -t rsa -C github的邮箱`

coder_dog@163.com

在ssh文件夹下，添加config

```
Host github.com
HostName ssh.github.com  # 这是最重要的部分
User git
Port 443
PreferredAuthentications publickey
IdentityFile ~/.ssh/id_rsa

```

