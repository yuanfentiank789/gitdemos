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
 git branch //查看当前所在分支

```