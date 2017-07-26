# Git

## 工作流程

### 创建或拉取
* git init
* git clone url

### 切分支
* git checkout -b dev

相当于2个命令，git branch dev，git checkout dev
先切分支，再干活

### 添加文件修改
* git add filepath
* git add -p

不建议用git add .

### 提交到本地
* git commit -m 'xxxx'

### 推送到远端分支
* git push origin dev

### 发起合并请求
在gitlab上操作，把url发给review的人

### 处理冲突
假设有冲突，gitlab上会有相应提示
需在本地处理完冲突后，再次推到gitlab上的分支上，才会提示可自动合并

切到master，更新本地master
* git checkout master
* git pull origin master

相当于2个命令，git fetch origin，git merge origin/master

切到分支，把master合并到分支
* git checkout dev
* git merge master
* git commit
* git push origin dev

### 其他命令
* git diff
* git log
* git log —pretty=oneline
* git reset —hard HEAD^

## 版本库
origin master
.git
stage

## .gitignore
