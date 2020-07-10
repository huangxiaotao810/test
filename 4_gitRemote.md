## 远程仓库



### 克隆仓库

```bash
$ git clone https://github.com/huangxiaotao810/git-skills.git
```



### 查看仓库

```bash
$ git remote -v
```





### 关联仓库

```bash
$ git remote add origin https://:@gitlab.cern.ch:8443/xiaotao/test.git
```



### 取消关联仓库

```bash
$ git remote remove origin
```



### 推送到仓库

```bash
$ git push origin <branch-name>
$ git push -u origin <branch-name> `
-u` 意同 --set-upstream，用以将本地库分支与远程库分支关联
```



### 拉取到本地仓库

```bash
$ git fetch origin master
$ git checkout origin/master
$ git merge origin/master

OR (pull == fetch + merge)

$ git pull origin master
```



### Create a new repository

```bash
$ git clone https://:@gitlab.cern.ch:8443/xiaotao/test.git
$ cd test
$ touch README.md
$ git add README.md
$ git commit -m "add README"
$ git push -u origin master
```



### Push an existing folder

```bash
$ cd existing_folder
$ git init
$ git remote add origin https://:@gitlab.cern.ch:8443/xiaotao/test.git
$ git add .
$ git commit -m "Initial commit"
$ git push -u origin master
```



### Push an existing Git repository

```bash
$ cd existing_repo
$ git remote rename origin old-origin
$ git remote add origin https://:@gitlab.cern.ch:8443/xiaotao/test.git
$ git push -u origin --all
$ git push -u origin --tags
```




