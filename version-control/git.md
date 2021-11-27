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
# this command will discard all your modification in staging area.
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

