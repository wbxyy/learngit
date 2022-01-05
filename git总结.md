### git 基础命令（重点）
`git init` 将当前目录初始化为git管理
`git add .` 将当前工作区文件提交到暂存区
`git commit -m "提交内容"` 提交暂存区的文件
`git status` 和 `git status -s` 查看工作区文件状态

### 能够使用 github 创建和维护远程仓库（重点）
能够配置 github 的 SSH 访问
能够将本地仓库上传到 github

### git 分支命令
分支简介：分支就是平行宇宙。多人协作开发时，每个人负责各自的功能分支，在功能完成后合并到主分支。

#### 查看（重点）
`git branch` 查看分支

#### 新增
`git branch 分支名` 创建新分支

#### 移动（重点）
`git checkout 分支名` 移动到指定分支

#### 新增并移动（重点）
`git checkout -b 分支名` 创建并移动到新分支

#### 合并
`git merge 分支名` 将指定分支合并到当前分支，一般用于将对应功能分支代码合并到主分支

#### 删除
`git branch -d 分支名` 删除指定分支，不能删除当前所处的分支
`git branch -D 分支名` 删除指定分支，未合并也会删除

### git 远程分支命令

#### 推送（重点）
`git push -u origin 本地分支名` 远程仓库分支名称保持一致时，可简写
`git push -u origin 本地分支名：远程分支名` 将本地分支推送到远程仓库


#### 查看
`git remote show origin` 查看远程分支列表

#### 下载
`git checkout 远程分支名` 追踪远程分支（下载远程分支）
`git checkout 本地分支名 origin/远程分支名` 追踪远程分支（下载远程分支并改名）

#### 更新
`git pull` 拉取远程分支上的最新代码，当前在哪个分支上运行该代码就拉取哪个分支的代码

#### 删除
`git push origin --delete 远程分支名` 删除远程分支