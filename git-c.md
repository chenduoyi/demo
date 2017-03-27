# 在本地创建一个文件夹, 用做工作区

# 在工作区起动git bash, git init, 初始化仓库
## git init

# 指定远程仓库, (指定需要拉取的远程仓库源头)
## git remote add origin[别名] https://github.com/username/remotename [仓库url]

# 获取远程仓库文件(update)
## git pull origin[仓库url, 可使用别名代替] master[分支,主分支为master]

# 本地操作仓库文件, 如新建文件夹, 修改文件等
## 新加入的文件或文件夹, 需要先将文件添加到暂存区
## git add [file1] [file2]
## 删除工作区文件
## git rm [file1] [file2]
## git 后撤一步, (比如说提交到暂存区后, 撤回到工作区), 记录指针回跳一步.
## git reset HEAD 

# 代码提交
## 提交暂存区到仓库
## -a => add,  -m => message
git commit -m [message] 
## 直接从工作区提交到仓库(提交前该文件已经在仓库中, 相当于直接覆盖上去)
git commit -a -m [message] 

# 查看信息
## 显示变更信息
## git status
## 显示当前分支的日志
## git log

# 将本地仓库文件推送到远程仓库,(commit)
## git push [remote] [branch]