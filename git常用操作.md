# git常用操作

https://blog.csdn.net/lshemail/article/details/115196971

## 远程仓库相关

新增一个 remote： `git remote add <shortname> <url>`

删除一个 remote：`git remote rm <shortname>`

查看当前仓库的 remote：`git remote -v`

## push 相关

**push -u**  第一次提交需要加 -u参数后，后面的提交就直接可以 git push

（1）以下命令将本地的 master 分支推送到 origin 主机的 master 分支。
git push origin master

（2）如果本地版本与远程版本有差异，但又要强制推送可以使用 --force 参数：
git push --force origin master

（3）删除主机的分支可以使用 --delete 参数，以下命令表示删除 origin 主机的 master 分支：
git push origin --delete master

## ssh 相关

**生成ssh密钥**  ssh-keygen -t rsa -C "这里换上你的邮箱"

## 代理相关

**use agent** git config --global http.proxy http://127.0.0.1:7890

**Unset agent** git config --global --unset http.proxy

## push demo

HTTPS  https://github.com/bigbitbox/myMallApp.git

SSH   git@github.com:bigbitbox/myMallApp.git

## Github token to IDEA

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
