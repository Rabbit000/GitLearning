# GitLearning
Upload local repository to Github

# 1.Set up SSH Key
1) Open Git bash.
2) Generate ssh keys:
      $ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
3) Copies the contents of the id_rsa.pub file to your clipboard:
      $ clip < ~/.ssh/id_rsa.pub 
4) Paste pub key in your github account's profile.
      Add new SSH key in "SSH and GPG keys".

# 2.Create a new repository
1) Enter repository name.
2) Enter discription.
3) Choose public or private. 
4) Initialize README file.
5) Choose programming language .gitignore file.
      no need to add .gitignore file manually.
6) Choose a license.
7) Create repository.

# 3.Synchronize local repository to Github.
1) $ git remote -v         #查看远端信息.
2) $ git remote add repository_name git_url       #添加远端信息.
3) $ git fetch repository_name master           #拉取远端版本仓库，不会跟本地的master进行merge.
4) $ git branch -v         #查看本地分支.
5) $ git branch -va        #查看所有分支（本地和远端）.
6) $ git merge -h          #查看merge帮助信息.
7) $ git merge --allow-unrelated-histories repository_name/master       #允许合并不相干的版本，一般采用“recursive”策略.
8) $ git push repository_name master      #同步本地仓库到Github.
  
