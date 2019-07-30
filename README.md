# GitLearning
Upload local repository to Github

# 1.Create a new repository
1) Enter repository name.
2) Enter discription.
3) Choose public or private. 
4) Initialize README file.
5) Choose programming language .gitignore file.
      no need to add .gitignore file manually.
6) Choose a license.
7) Create repository.

# 2.Synchronize local repository to Github.
$ git remote -v  #查看远端信息
$ git remote add <name> <url> #添加远端信息
$ git fetch <name> master #拉取远端版本仓库，不会跟本地的master进行merge
$ git branch -v #查看本地分支
$ git branch -va #查看所有分支（本地和远端）
$ git merge -h #查看merge帮助信息
$ git merge --allow-unrelated-histories <name>/master #允许合并不相干的版本，一般采用“recursive”策略
$ git push <name> master #同步本地仓库到Github
  
