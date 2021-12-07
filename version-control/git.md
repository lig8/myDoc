# git 使用简介

## 0、参考文档

- [如何高效使用github](https://www.yangzhiping.com/tech/github.html)

- [git简明指南](http://rogerdudler.github.io/git-guide/index.zh.html)

123

## 0、访问权限

### a、personal access token方式

- [官方文档](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) 
- [如何存贮在.git中](https://www.jianshu.com/p/e5a3530cb021)

- [如何存贮在windows凭证中](https://segmentfault.com/a/1190000040544939?utm_source=sf-similar-article)

### b、SSH key方式

- [官方文档](https://docs.github.com/cn/authentication/connecting-to-github-with-ssh)
- [多密钥管理](https://www.cnblogs.com/logchen/p/10543808.html)

## 1、git基本设置

### a、设置git bash支持中文显示

```bash
# git bash support chinese
git config --global core.quotepath false
```



## 2、git 最常用的6个命令

- [merge与rebase的区别](http://gitbook.liuhui998.com/4_2.html)
- [merge noff](https://www.cnblogs.com/xueweihan/p/5743327.html)
- [分支与合并](http://gitbook.liuhui998.com/3_3.html)

![](https://raw.githubusercontent.com/lig8/myData/main/programming/git/git1.png)

![](https://raw.githubusercontent.com/lig8/myData/main/programming/git/git5.jpg)

```bash
# add all modified files to staging area.
git add -A

# commit all modified files in staging area to local Repository
git commit -m 'my comments'
# add commit comments in external editor.
git commit -a

# push modified files from local Repository to remote Repository
git push

# push your code to other branch
git push origin branch_name

# undo modification in staging area. 
# this command will discard all your modification in staging area.
git restore --staged .

#update local repository to latest code.
git pull



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



```bash
git reset HEAD
git reset --soft --hard
git tag -d
git clean -nxdf（查看要删除的文件及目录，确认无误后再使用下面的命令进行删除）
git checkout . && git clean -xdf
git reset 删除的是已跟踪的文件，将已commit的回退。
git clean 删除的是未跟踪的文件
git checkout . #本地所有修改的。没有的提交的，都返回到原来的状态
git stash #把所有没有提交的修改暂存到stash里面。可用git stash pop回复。
 
git reset --hard HASH #返回到某个节点，不保留修改，已有的改动会丢失。
git reset --soft HASH #返回到某个节点, 保留修改，已有的改动会保留，在未提交中，git status或git diff可看。
 
git clean -df #返回到某个节点，（未跟踪文件的删除）
git clean 参数
 -n 不实际删除，只是进行演练，展示将要进行的操作，有哪些文件将要被删除。（可先使用该命令参数，然后再决定是否执行）
 -f 删除文件
 -i 显示将要删除的文件
 -d 递归删除目录及文件（未跟踪的）
 -q 仅显示错误，成功删除的文件不显示
 
 
 回退push过的代码：
1. git log
2. git reset --soft 43dc0de914173a1a8793a7eac31dbb26057bbee4
3. git push origin branch_name --force


删除分支：
git branch -a
git branch -D branch_name
git push origin --delete branch_name  

删除tag：
git tag -l
git tag -d tag_name
git push origin :refs/tags/tag_name

push tags:
git push origin --tags
git push origin tag_name

```



#### 新建代码仓库

* 首先要在服务器上新建一个空仓库，不要有任何东西    https://gitee.com/lig0/pyStudy.git

```bash
cd pyStudy
git init
git add -A
git commit -m "init repository"
git remote add origin https://gitee.com/lig0/pyStudy.git
git push -u origin master
```







