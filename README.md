# CS_learing
## GIT总结
### 操作本仓库的命令
  - 1 在当前目录创建版本库：
  `git init `
  - 2 添加的单个文件到暂存区
  ` git add readme.txt`
  - 3 把文件提交到仓库
  ` git commit -m "first commit"`
  - 掌握工作区的状态
  ` git status`
  - 如果git status 告诉你又文件被修改过，查看修改内容
  ` git diff`
  - 回退版本
  ` git reset --hard commit_id`
  - 查看提交历史
  ` git log`
  - 要重返未来，查看命令历史，来确定回到哪个未来
  ` git reflog`
  - 当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时
  ` git checkout -- file`
  当乱改了工作区某个文件的内容，还添加到了暂存区，想丢弃修改，分两步。
  ` git reset HEAD <file>` 然后按照上一个命令操作
  - 删除版本库的一个文件
  ` git rm`
### 推送本地版本库到github
  - 关联一个远程库
  ` git remote add origin git@server-name:path/repo-name.git`
  - 第一次推送master分支的所有内容
  ` git push -u origin master`
  - 推送最新修改
  ` git push origin master`  
### 分支
  - 查看分支
  ` git branch`
  - 创建分支
  ` git branch name`
  - 切换分支
  ` git checkout name`
  - 创建并且同时切换分支
  ` git checkout -b name`
  - 合并某分支到当前分支
  ` git merge name`
  - 删除分支
  `git branch -d name`
  - 查看分支合并图
  ` git log --graph`
  
