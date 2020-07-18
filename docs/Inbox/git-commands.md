---
title: "Git Commands"
layout: page
date: 2018-09-28 00:00
---

### Git 克隆某分支
`git clone -b <branch> <repo>`

### Git 自动纠错
`git config --global help.autocorrect 1`
比如 `git comit` 纠正为 `git commit`

### Git 推送上游
`git push -u origin master` 
`-u, –set-upstream`
代表的是默认推送的地方，这里就是默认以后 git pull 和 git push 的分支

### Git 删除远程分支

首先查看远程分支

```bash
git branch -r
```

然后把 `branch-name` 替换为要删除的远程分支名字

```bash
git branch -r -d origin/branch-name
git push origin :branch-name
```

### Git 修改历史提交 Commit 信息

```bash
// 使用 git rebase 可以修改历史 Commit 信息
git rebase -i '<hash_id>^'
```



