https://github.com/zxjajin/git-demo.git

#### SSH：git@github.com:zxjajin/git-demo.git

### Git常用命令

|                  命令名称                  |                           作用                           |
| :----------------------------------------: | :------------------------------------------------------: |
|    git config --global user.name 用户名    |                       设置用户签名                       |
|    git config --global user.email 邮箱     |                       设置用户签名                       |
|              git ini（重点）               |                       初始化本地库                       |
|             git status（重点）             |                      查看本地库状态                      |
|           git add 文件名（重点）           |                       添加到暂存区                       |
|           git rm --cached 文件名           |                      删除暂存区文件                      |
|  git commit -m "日志信息" 文件名（重点）   |                       提交到本地库                       |
|             git reflog（重点）             |                       查看历史记录                       |
|                  git log                   |                     查看版本详细信息                     |
|      get reset --hard 版本号（重点）       |                         版本穿梭                         |
|             git branch 分支名              |                         创建分支                         |
|               git branch -v                |                         查看分支                         |
|            git checkout 分支名             |                         切换分支                         |
|          git merge 分支名（重点）          |               把指定的分支合并到当前分支上               |
|               git remote -v                |                 查看当前所有远程地址别名                 |
|        git remote add 别名 远程地址        |                          起别名                          |
|         git push 别名 分支（重点）         |              推送本地分支上的内容到远程仓库              |
|         git clone 远程地址（重点）         |                将远程仓库的内容克隆到本地                |
| git pull 远程库地址别名 远程分支名（重点） | 将远程仓库对应分支最新内容拉下来后与当前本地分支直接合并 |

### Liunx命令

#### vim 文件名：创建文件或者修改文件

#### cat 文件名：查看文件内容

#### :wq回车保存文件

#### :q不保存退出文件

#### yy 复制当前行

#### dd 删除当前行

#### pp 粘贴到当前行

SSH免密登录具体操作如下： --进入当前用户的家目录 Layne@LAPTOP-Layne MINGW64 /d/Git-Space/SH0720 (master) $ cd --删除.ssh 目录

家目录打开命令行输入；ssh-keygen -t rsa -C 邮箱名字

![image-20230103144033130](C:\Users\阿金\AppData\Roaming\Typora\typora-user-images\image-20230103144033130.png)

这个是由于Git默认开启了SSL验证，关闭即可；

解决方法执行

git config --global http.sslVerify false
