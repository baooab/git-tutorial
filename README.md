# test

a test repo.

一、常用命令

```
# 查看所有分支（包括远程分支）
git branch -a
```

```
# 新建分支 v0.0.1 并切换（分支已有，会报错，命令执行失败）
git checkout -b v0.0.1
```

```
# 将本地的新分支推送到远程仓库
git push --set-upstream origin v0.0.1
```

```
# 删除本地分支 v0.0.1
git branch -d v0.0.1
# 删除远程分支 v0.0.1
git push origin --delete v0.0.1
```