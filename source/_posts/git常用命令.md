---
title: git常用命令
date: 2017-07-13 17:18:48
tags: git
categories: web
---

## 拉取远程仓库并创建自己的分支

1. 克隆远程仓库到本地 `git clone git://xxxx.git` 或者 `git clone http:// xxxx.git`
2. 查看分支 `git branch -a`
3. 切换分支 `git checkout xxx`
4. 创建分支 `git branch xxx` 
5. 创建分支并切换到此分支 `git checkout -b xxx`

## 提交代码

1. 从远端更新到本地 `git pull origin xxx`
2. 查看状态 `git status`
3. 添加到暂存区 `git add .` 或者 `git add xxx`
4. 提交当前暂存区代码 `git commit -m "本次提交注释"`
5. 提交到远端仓库 `git push origin xxx`

## 合并分支

1. 合并其他分支 `git merge origin/xxx`
2. 解决冲突后 重新add

## 其他（很重要！！）
1. 删除分支 `git branch -d xxx` (d只能删除已经参与过merge的分支)
2. 强制删除分支 `git branch -D xxx`
3. 查看操作记录 `git log`
4. 重置回上一版本 `git reset --hard head` (超级有用，误操作之后恢复线上版本)
5. 记录所有head的历史 `git reflog` (可找回reset丢掉的commit)

