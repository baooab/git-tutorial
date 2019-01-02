# Git Commands

Git commands list.

```
# 查看所有分支（包括远程分支）
git branch -a
```

```
# 新建分支 v0.0.1 并切换（分支已有，会报错，命令执行失败）
git checkout -b v0.0.1

# 将本地的新分支推送到远程仓库
git push --set-upstream origin v0.0.1
```

```
# 删除本地分支 v0.0.1
git branch -d v0.0.1

# 删除远程分支 v0.0.1
git push origin --delete v0.0.1
```

```
# 获取远程所有分支列表
git fetch

# 获取远程分支 v0.0.1
git fetch origin v0.0.1

# 在远程分支 v0.0.1 的基础上，创建一个新的本地分支 v0.0.1
git checkout -b v0.0.1 origin/v0.0.1
```

参考资料

1. [連猴子都能懂的Git入門指南](https://backlog.com/git-tutorial/tw/stepup/stepup2_2.html)
2. [Git远程操作详解](http://www.ruanyifeng.com/blog/2014/06/git_remote.html), by 阮一峰