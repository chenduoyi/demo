# git add深入讲解
## 添加新文件
touch t.txt

## 删除文件
git rm t.txt

## 编辑文件(增加内容,删除内容,修改内容)
vim t.txt 后对文件内容进行增加,删除,修改, 然后保存退出

## 文件改名
git mv t.txt tt.txt

## 文件移动
git mv t.txt ./doc

## 文件夹的操作(添加,删除,改名,移动)
mkdir test
只添加目录, 而没有写入文件, 不会被追踪
git mv test test2
git rm -rf test2

## 一个文件多个提交
git 的提交, 不是基于文件的, 而是基于变更的. 可以按变更逐个提交
git add -p 文件名
Stage this hunk [y,n,q,a,d,/,e,?]?
y 提交保存
n 不提交保存

