# Git操作详解以及在VScode中的使用

[![鬼木士](https://picx.zhimg.com/v2-fade060a30524a50d420ee8ad087fcf1_l.jpg?source=172ae18b)](https://www.zhihu.com/people/ghowoght)

[鬼木士](https://www.zhihu.com/people/ghowoght)

一定会没问题的

关注他

156 人赞同了该文章

我们先理清**Git和Github的区别**，Git是个版本控制的工具，用来管理本地的代码工程，它可以记录代码内容的变更；而Github是一个代码托管平台，我们可以使用Git将本地代码上传到Github。

**为什么要学Git**，上面说到Git是一个版本控制工具，它可以记录代码内容的变更，方便我们对项目的管理，它主要有以下的用途：

- **代码备份**

举一个简单的例子，写好一个程序后，想要再加一个新功能，添加这个新功能需要对很多个文件进行改动。但是添加完这个功能后发现，这个新功能是个坑，然后就会想着回退到上一个版本，这时候如果有备份还好，没有备份的话就得ctrl+z，甚至要按照自己的记忆恢复以前的版本

如果使用Git就好办了，直接使用git切换下版本或者分支就可以了。

当然先备份一下原始代码，然后在上面改，也是一个很简单且有效的方法，但是随着新功能的增加，程序所占用的内存越来越大，而且每个版本间的区别很难直观看出，这不利于我们对项目的管理

- **多人协作**

假设要做一个项目，这个项目中有多个功能，大多数情况下，我们不可能一个功能一个功能地做，而是进行团队分工，多个功能同步进行，这时候如果没有使用Git进行版本控制，那么在将这些功能统合时将会出现很大的问题

- **以后工作的需要**

目前很多公司都在用Git进行项目管理，学会Git对以后的工作还是很有好处的

本文将介绍Git的基本工作流程，以及这些流程对应的命令行指令，最后对VScode中内置的Git进行介绍和演示

## Git安装

Git在Windows上和在Linux上的使用方式基本无差别，所以本文中的演示主要在Windows上进行

### Windows

在[这里](https://link.zhihu.com/?target=https%3A//git-scm.com/downloads)可以下载最新版的Git，然后一路Next即可

### Ubuntu

```bash
sudo apt-get install git
```

## Git工作流程

基本工作流程图：

![img](https://pic1.zhimg.com/80/v2-cd9ae639fa7ba273ffc3753037629ee0_1440w.webp)

- 工作区(Workspace)：平时存放项目代码的地方
- 暂存区(Index/Stage)：用于临时存放改动信息
- 本地仓库(Repository)：存放所有提交的版本数据
- 远程仓库(Remote)：托管代码的服务器，比如我们经常用的Github就是个代码托管平台

git的基本工作流程如下：

1. 在工作区中添加、修改文件
2. 将工作区中需要进行版本管理的文件放入暂存区
3. 将暂存区的文件提交到git本地仓库
4. (**optional**)将本地仓库推送到远程仓库

为了方便以后的学习和工作，不建议直接使用GUI来操作Git，下面将针对上面的工作流程介绍一些常用的Git命令行指令，这些指令是比较简单的，敲熟练之后再上手GUI版本的Git就相当容易了

### 初始化

初始化git，有两种方式：

```bash
# 方式一:本地生成一个git
git init
# 方式二:从远端克隆一个仓库
git clone https://gitee.com/xxxxxx/xx.git
```

基本配置

```bash
# 配置用户名
git config --global user.name "name"
# 配置邮箱
git config --global user.email "name@mail.com"
```

删除远程仓库

```bash
git remote rm origin
```

添加远程仓库

```bash
git remote add origin https://gitee.com/xxxxxx/xx.git
```

### 推送至远程仓库

将已修改文件添加至暂存区

```bash
git add dir/filename # 添加指定文件
git add . # 添加所有已修改文件
```

将暂存区的改动提交到本地的版本库，使用`git commit`命令我们就会在本地版本库生成一个40位的哈希值，用于版本回退

```bash
git commit -m "message" # message就是本次提交的简要说明
```

本地上传，注意在推送前需要先从远程拉取

```bash
git push -u origin master # master可以更换为其他分支
```

### 从远程仓库拉取

更新本地：

```bash
git pull origin master # master可以更换为其他分支
```

### 分支管理

分支管理是版本控制中一个很重要的内容，在Git中主要有切换/创建分支(checkout)、合并分支(merge)两个指令

下面是部分分支操作的指令和图示，圆圈○表示一个提交(commit)记录，矩形表示分支，它指向一个提交记录，由这个记录可以遍历之前所有的提交记录

首先初始化了一个git，这个git中只有一个`master`分支，包含两个commit记录

![img](https://pic1.zhimg.com/80/v2-e4f88ddafff72af14821b1f014280134_1440w.webp)

现在我们创建一个新分支，命名为`develop`：

```bash
git checkout -b develop # 表示创建并切换到develop分支
```

![img](https://pic4.zhimg.com/80/v2-d5504a1b7cdc368a01b900f013084527_1440w.webp)

此时`master`分支和`develop`分支都指向C1这个提交记录。我们分别在这两个分支上进行修改并提交：

```bash
git commit
git checkout master # 切换到master分支
git commit
```

![img](https://pic1.zhimg.com/80/v2-afdb0ab985d5784b4e063938963ca970_1440w.webp)

可以看到`master`分支和`develop`分支指向了不同的提交记录，接下来我们将`develop`分支合并到`master`分支中

```bash
git merge develop
```

![img](https://pic2.zhimg.com/80/v2-991bc8e3e03d37d6d148df5981090bad_1440w.webp)

执行上面的指令后，产生了一个新的提交记录C4，由C4我们可以遍历之前所有的提交记录，但是此时`master`分支和`develop`分支仍然指向不同的提交记录。继续切换到`develop`分支，将`master`分支合并到`develop`分支中：

```bash
git checkout develop
git merge master
```

![img](https://pic3.zhimg.com/80/v2-c9489a4cc8cf75238823b852a743a5c2_1440w.webp)

### 打标签

使用Git可以给指定提交打上标签，用来突出显示这个提交，比如将提交标记为v1.0、v2.0，等等

- **列举标签**

使用如下命令即可列出所有标签

```bash
git tag
```

当标签太多时，可以使用如下指令列出包含指定字符的标签

```bash
git tag -l "v1.*"
```

- **创建标签**

添加-a选项即可创建标签，如下：

```bash
git tag -a v1.0 -m "version 1.0"
```

如上命令即可为当前提交创建一个标签，标签名为v1.0，-m选项后就是该标签的附注信息

- **推送标签**

只使用git push命令在默认情况下不会将标签推送到 远程仓库，在创建标签后需要执行如下命令将指定标签推送到远程仓库：

```bash
git push origin <tagname>
```

如果要推送多个新标签，可以使用git push的--tags选项将所有标签推送到远程仓库：

```bash
git push origin --tags
```

- **删除标签**

使用git tag的-d选项即可删掉本地仓库上的指定标签，如下：

```bash
git tag -d <tagname>
```

但是该指令不会删除远程仓库中的标签 ，还需要使用如下命令来更新远程仓库：

```bash
git push remote :refs/tags/<tagname>
```

- **切换标签**

使用git checkout <tagname>指令即可将git仓库的HEAD指针指向标签所在的提交，如下：

```bash
git checkout v1.0
```

## VScode中的Git使用

### 本地仓库操作

当对仓库已经被跟踪的文件进行修改的时候，会有三种文件状态。如图：

![img](https://pic3.zhimg.com/80/v2-ef4f2f4e1453c1311cf6ffb0f045057a_1440w.webp)

- M(Modify)，表示该文件存在修改
- D(Delete)，表示该文件被删除
- U(Update)，表示该文件是新添加的

选中文件即可查看已进行的修改

![img](https://pic1.zhimg.com/80/v2-21bd732c279178de83fa5d46fd6092a4_1440w.webp)

接下来可以对这些更改进行处理，可以选择放弃修改或者保存修改，选择放弃修改的话，该文件就会回退到上次保存的版本

![img](https://pic4.zhimg.com/80/v2-cf629edd3ff909f59eb01649d91caf6b_1440w.webp)

也可以点击上面的图标对所有更改进行处理

![img](https://pic1.zhimg.com/80/v2-99bad335d95735ca5b3bdcbd411bff30_1440w.webp)

我们选择保存所有修改，所有已修改文件就会保存到暂存区，对应的git命令为`git add .`

接下来将暂存区的改动提交到本地的版本库，点击上方的“√”，对应git命令`git commit`，然后添加message即可

![img](https://pic2.zhimg.com/80/v2-e0396dff6e22c3363f64a7f640233455_1440w.webp)

这时候所有的修改就已经处理完毕了

![img](https://pic2.zhimg.com/80/v2-557dcf3b8c86daa348daa9fca6f8c5d1_1440w.webp)

### 推送到远程仓库

将本地仓库上的修改推送到远程仓库，对应git命令`git push`

![img](https://pic3.zhimg.com/80/v2-7f0d54b382afc8f6059c83de4d7c7022_1440w.webp)

一般情况下，VScode会弹出账号密码的输入窗口进行登录

最后查看远程仓库：

![img](https://pic2.zhimg.com/80/v2-760189c2e52dbdcd29962717d0270561_1440w.webp)

### 从远程仓库拉取

与推送类似，如图，对应git命令`git pull`

![img](https://pic1.zhimg.com/80/v2-5742bd638076376dea0eeea548850f34_1440w.webp)

### 分支管理

VScode可以直接在左下角创建/切换分

![img](https://pic3.zhimg.com/80/v2-675d844f01c011c1a0a422379dd42f6e_1440w.webp)

合并分支

![img](https://pic3.zhimg.com/80/v2-9447b8ffaeca8879a8c819f7834c1ec2_1440w.webp)

如果待合并的分支上的修改和master没有冲突，就可以直接合并。但是在多人协作时常常会出现两个分支存在不同修改的情况，这时候就要对这些冲突进行处理：

![img](https://pic3.zhimg.com/80/v2-98ef03a3554f080504c3f125179d3306_1440w.webp)

### GitLens插件

使用VScode自带的git支持对于个人开发来说已经足够了，但是在应对团队协作时的文件冲突时还略显不足，这时候我们可以借助VScode中的GitLens插件，使用方法详见[git源代码管理插件GitLens](https://link.zhihu.com/?target=https%3A//www.jianshu.com/p/a91cb8a2e55d)

## 参考

[Git 分支管理最佳实践developer.ibm.com/zh/articles/j-lo-git-mange/](https://link.zhihu.com/?target=https%3A//developer.ibm.com/zh/articles/j-lo-git-mange/)

[Git教程www.liaoxuefeng.com/wiki/896043488029600![img](https://pic3.zhimg.com/v2-23dad9e5cdf40848a5ad1c72bf5de2c6_180x120.jpg)](https://link.zhihu.com/?target=https%3A//www.liaoxuefeng.com/wiki/896043488029600)

[VScode 结合git的全面使用流程，再也不用记住git的命令了！blog.csdn.net/weixin_43314519/article/details/107572206![img](https://pic3.zhimg.com/v2-ee64702a944d84466a59ea45c2f45e2a_ipico.jpg)](https://link.zhihu.com/?target=https%3A//blog.csdn.net/weixin_43314519/article/details/107572206)

[Learn Git Branchingoschina.gitee.io/learn-git-branching/![img](https://pic1.zhimg.com/v2-8e7132076f76bc1c65eb1f41d15e1aa8_180x120.jpg)](https://link.zhihu.com/?target=https%3A//oschina.gitee.io/learn-git-branching/)



编辑于 2022-02-02 15:18