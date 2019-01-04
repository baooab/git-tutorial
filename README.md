# Git 远程指令

常用远程指令列表：

```
# 查看所有分支（包括远程分支）
git branch -a
```

```
# 新建分支 v0.0.1 并切换（如果分支已有，该命令会报错，执行失败）
git checkout -b v0.0.1
# 上面的命令等同于
# git branch v0.0.1
# git checkout v0.0.1

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

# 在远程分支 v0.0.1 的基础上，创建本地分支 v0.0.1
git checkout -b v0.0.1 origin/v0.0.1
```

```
# 打标签
git tag v0.0.1

# 推送到远程仓库
git push origin --tags

# 删除本地标签
git tag -d v0.0.1

# 删除远程标签
git push origin :refs/tags/v0.0.1
```

参考资料：

1. [連猴子都能懂的Git入門指南](https://backlog.com/git-tutorial/tw/stepup/stepup2_2.html)
2. [Git远程操作详解](http://www.ruanyifeng.com/blog/2014/06/git_remote.html), by 阮一峰
3. [git 打标签并推送tag到托管服务器](http://yijiebuyi.com/blog/007269d04d5096d9397ce3daf9d84c48.html), by 一介布衣