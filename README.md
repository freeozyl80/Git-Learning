# Git-Learning

## Learn Everything about Git

### Git clone

使用 git clone 拷贝一个 Git 仓库到本地，让自己能够查看该项目，或者进行修改。
如果你需要与他人合作一个项目，或者想要复制一个项目，看看代码，你就可以克隆那个项目。 

执行命令：

> git clone [url]


### Git add

git add 命令可将该文件添加到缓存，如我们添加以下两个文件：

> git add [file]


### Git status

git status 命令用于查看项目的当前状态。


### Git commit

git commit 用于 提交所有改动

> git commit -a 用于跳过add命令


### Git log  （ps: q为退出键）

git log 用于显示所有提交历史记录

参数 ： -n 显示前N条


### Git remote 

git remote 显示当前所有的远程库

> git remote add (name)(.git) // 添加远程库文件

> git remote show (name) // 显示远程库具体信息


### Git push

git push 用于将本地分支的更新，推送到远程主机上

> git push (name)(本地分支名):(远程分支名)

// 如果省略远程分支名，则表示将本地分支推送与之存在"追踪关系"的远程分支（通常两者同名），如果该远程分支不存在，则会被新建。

### Git 回滚

> git checkout -- file；
// 撤销对工作区修改；这个命令是以最新的存储时间节点（add和commit）为参照，覆盖工作区对应文件file；这个命令改变的是工作区

>git reset HEAD -- file；
// 清空add命令向暂存区提交的关于file文件的修改（Ustage）；这个命令仅改变暂存区，并不改变工作区，这意味着在无任何其他操作的情况下，工作区中的实际文件同该命令运行之前无任何变化，一般情况下都是先进行reset HEAD 以后 再次进行 checkout实现清空
