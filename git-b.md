# 新建代码仓库
## 在当前目录新建一个Git代码库
git init
## 下载一个项目和它的整个代码历史
url格式 https://github.com/[username]/reposName
git clone [url]

# 添加删除文件
## 添加指定文件到暂存区
git add [file1] [file2]
## 删除工作区文件
git rm [file1] [file2]
## 改名文件, 并且将这个改名放入暂存区
git mv [file-origin] [file-rename]

# 代码提交
## 提交暂存区到仓库
## -a => add -m => message
git commit -m [message] 
## 直接从工作区提交到仓库(提交前该文件已经在仓库中, 相当于直接覆盖上去)
git commit -a -m [message] 

# 查看信息
## 显示变更信息
git status
## 显示当前分支的历史版本
git log 

# 同步远程仓库
## 增加远程仓库 
## remote 即远程仓库, shortname 别名, url 远程仓库的地址, branch 分支, 主分支为 master
git remote add [shortname] [url]
## 将远程仓库的提交拉下到本地
git pull [remote] [branch]
## 将本地的提交推送到远程仓库
git push [remote] [branch]

