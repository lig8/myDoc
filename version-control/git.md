# git 使用简介

## 1、git基本设置

```bash
# git bash support chinese
git config --global core.quotepath false
```



## 2、git 最常用的6个命令

![](https://raw.githubusercontent.com/lig8/myData/main/programming/git/git1.png)

![](https://raw.githubusercontent.com/lig8/myData/main/programming/git/git5.jpg)

```bash
# add all modified files to staging area.
git add -A

# commit all modified files in staging area to local Repository
git commit -m 'my comments'

# push modified files from local Repository to remote Repository
git push

# undo modification in staging area. 
git restore --staged .

```

![](https://raw.githubusercontent.com/lig8/myData/main/programming/git/git7.png)

![](https://raw.githubusercontent.com/lig8/myData/main/programming/git/git6.png)




```bash
# git undo modification from local Repository
git reset --soft HEAD^
git reset --hard HEAD^
git reste --mixed HEAD^

```

![](https://raw.githubusercontent.com/lig8/myData/main/programming/git/git2.png)

```bash
# git get code from Remote
git clone
git fetch
git pull
```



![](https://raw.githubusercontent.com/lig8/myData/main/programming/git/git4.jpg)

![](https://raw.githubusercontent.com/lig8/myData/main/programming/git/git3.png)

