#### 一些HTML/CSS/JS的练习代码

#### Git 学习笔记
```bash
git clone href filename
cd filename
git add file/.
git rm --cached file
git commit -m "message"
git commit --amend
git tag -a version_name #with message
git tag -d version_name
git tag version
git log
git log --decorate
git branch # show branch
git branch branch_name # new branch
git checkout branch_name # switch branch
git checkout -b branch_name # new branch + switch
git branch -d branch_name # clean commit delete branch not in
git branch -D branch_name # force delete branch
git merge
git revert commitid # revert commit 
```
- 基本操作
```bash
# 在当前目录新建一个Git代码库
git init                        
# 新建一个目录，将其初始化为Git代码库
git init <project-name>         
# clone git仓库
git clone <git-hub-url>  
# [高阶用法] clone git仓库并且制定分支
git clone <url> -b <branch>
# 已当前分支为基础，创建daily/0.0.1分支
git checkout -b daily/0.0.1
# 查看本地分支及远端分支
git branch -la 
# 强制删除本地分支
git branch -D [branchName]
# 删除已经Merge过的分支
git branch -d [branchName]
# 如何删除远端多余分支
# 大多数情况remote_name为origin
git push -delete <remote_name> <branchName> 
# 查看当前工作区改动点
git diff                               
# 提交hash1和hash2的差异
git diff commit_hash1 commit_hash2 
# 分支a和b的差异
git diff branch_a branch_b   
# 当前改动文件
git status     
# 查看提交历史
git log                
# 提交历史缩减一行查看，主要是提交Hash值
git log --pretty=oneline
# 添加子模块
git submodule add 仓库地址
# 更新子模块
git submodule update --remote 模块名称
## 删除子模块
1. git rm --cached 模块名称
2. 删除 .gitmodules 下相应子模块信息
3. 删除 .git/config 下相应子模块信息
```