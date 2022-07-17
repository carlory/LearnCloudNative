# Git Tips

## 增加远程仓库

```sh
git remote add upstream <remote-url>
```

## 创建并切换到本地分支

```sh
git checkout -b <branch-name>
```

## 放弃工作区的修改

```sh
git checkout <file-name>
```

放弃所有修改：
```sh
git checkout .
```

## 同步上游仓库的变化

```sh
git fetch upstream master
git rebase upstream/master
```

当发生冲突时, 需手动解决, 解决后:

```sh
git add .
git rebase --continue
```

## 修改作者名

```sh
git commit --amend --author='Author Name <email@address.com>'
```

## 远程删除了分支本地也想删除

```sh
git remote prune origin
```

## 更多

- [git-tips](https://github.com/521xueweihan/git-tips)