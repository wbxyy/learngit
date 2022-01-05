### git 基础命令
`git init` 将当前目录初始化为git管理
`git add .` 将当前工作区文件提交到暂存区
`git commit -m "提交内容"` 提交暂存区的文件
`git status` 和 `git status -s` 查看工作区文件状态

### git 分支命令
分支简介：分支就是平行宇宙。多人协作开发时，每个人负责各自的功能分支，在功能完成后合并到主分支。
`git branch` 查看分支
`git branch 分支名` 创建新分支
`git checkout 分支名` 移动到指定分支
`git checkout -b 分支名` 创建并移动到新分支

`git merge 分支名` 将指定分支合并到当前分支，一般用于将对应功能分支代码合并到主分支
`git branch -d 分支名` 删除指定分支，不能删除当前所处的分支

`git push -u origin 本地分支名：远程分支名` 将本地分支推送到远程仓库
`git push -u origin 本地分支名` 远程仓库分支名称保持一致时，可简写

`git remote show origin` 查看远程分支列表

`git checkout 远程分支名` 追踪远程分支（下载远程分支）
`git checkout 本地分支名 origin/远程分支名` 追踪远程分支（下载远程分支并改名）