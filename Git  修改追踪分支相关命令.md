##  Git  修改追踪分支相关命令

~~~shell
# 查看本地分支和远程分支追踪关系
git branch -vv
# 切换分支
git checkout master
# 将branch-name分支追踪远程分支origin/branch-name
git branch --set-upstream branch-name origin/branch-name
# 将当前分支跟踪origin/master
git branch -u origin/master
# 在远程分支的基础上建立develop分支，并且让develop分支追踪origin/develop远程分支
git checkout -b develop origin/develop
# 克隆时自动将创建好的master分支追踪origin/master分支
git clone 服务器地址

# 设定当前分支的 FETCH_HEAD' 为远程服务器的branch1分支`.
git fetch origin branch1
# 取所有分支
git fetch
# 取特定分支
git fetch 仓库名 分支名

# git查看远程仓库地址命令
git remote -v
# 修改远程仓库
git remote rm origin
git remote add origin [url]
git remote add pb git://github.com/paulboone/ticgit.git
# 设置新的远程仓库
git remote origin set-url [url]  

# 使A local仓库和远程upstream仓库的master分支同步
# git fetch origin guangda-dev
# git rebase 
$ git fetch upstream
$ git rebase upstream/master

~~~

