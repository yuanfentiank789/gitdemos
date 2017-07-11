# 初始化git仓库
## 初始化git仓库并关联到远程仓库
```
echo "# gitdemos" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:yuanfentiank789/gitdemos.git
git push -u origin master
```

## 关联本地仓库到远程github
```
git remote add origin git@github.com:yuanfentiank789/gitdemos.git
git push -u origin master
```

# 分支管理

```
查看所在分支：git branch

创建本地分支：git branch <name>

切换到本地分支：git checkout <name>

关联本地分支到远程分支:git push --set-upstream origin dev

创建+切换本地分支：git checkout -b <name>

check远程分支并切换到该分支：git checkout -b 本地分支名 远程分支名，eg:git checkout -b master origin/master

合并某分支到当前分支：git merge <name>

删除分支(大D强制删除)：git branch -d <name>

删除远程分支：git push origin --delete test

git重命名本地分支：git branch -m old-local-branch-name new-local-branch-name

```

# TAG管理

>git标签，tag就是一个容易记住的有意义的名字，它跟某个commit id绑在一起.切换到需要打标签的分支上，默认打在最新提交的commit上.

```
在当前分支最新提交上创建一个tag：git tag v1.0
指定commit id一个tag：git tag v0.9 6224937
查看所有tag:git tag
查看指定tag信息：git show <tagname>
删除tag:git tag -d v1.0
push tag到远程(默认只在本地)：git push origin v1.0
push所有tag:git push origin --tags

删除远程tag：
step1,先从本地删除：git tag -d v0.9；
step2.删除远程tag：git push origin :refs/tags/v0.9

```

# 版本回退

> 每提交一个新版本，实际上Git就会把它们自动串成一条时间线.现在我们启动时光穿梭机,在历史版本间穿梭。

```
查看提交记录：git log
简化git log输出：git log --pretty=oneline

```
