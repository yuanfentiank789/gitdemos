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

删除分支：git branch -d <name>

git重命名本地分支：git branch -m old-local-branch-name new-local-branch-name

```