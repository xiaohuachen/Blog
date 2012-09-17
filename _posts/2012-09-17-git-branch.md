##创建分支并切换到改分支

> `git checkout -b iss53`

> *相当于执行下面这两条命令*

> `git branch iss53`


> `git checkout iss53`

##切换分支


> `git checkout master`

##删除分支

> `git branch -d hotfix`

> *用大写的删除选项 -D 强制执行*

##合并分支

> *通常是回到master分支上运行如下命令*

> `git checkout master`

> `git merge iss53`

##调用一个可视化的合并工具
> `git mergetool`

##查看哪些分支已被并入当前分支
> `git branch --merge`

##查看尚未合并的工作
> `git branch --no-merged `

##远程分支
> `(远程仓库名)/(分支名) `

> *假设你们团队有个地址为 git.ourcompany.com 的 Git 服务器。如果你从这里克隆，Git 会自动为你将此远程仓库命名为 origin，并下载其中所有的数据，建立一个指向它的 master 分支的指针，在本地命名为 origin/master，但你无法在本地更改其数据。接着，Git 建立一个属于你自己的本地 master 分支，始于 origin 上 master 分支相同的位置，你可以就此开始工作。一次 Git 克隆会建立你自己的本地分支 master 和远程分支 origin/master，它们都指向 origin/master 分支的最后一次提交。如果你在本地 master 分支做了些改动，与此同时，其他人向 git.ourcompany.com 推送了他们的更新，那么服务器上的 master 分支就会向前推进，而于此同时，你在本地的提交历史正朝向不同方向发展。不过只要你不和服务器通讯，你的 origin/master 指针仍然保持原位不会移动。可以运行 git fetch origin 来同步远程服务器上的数据到本地。该命令首先找到 origin 是哪个服务器（本例为 git.ourcompany.com），从上面获取你尚未拥有的数据，更新你本地的数据库，然后把 origin/master 的指针移到它最新的位置上。在克隆仓库时，Git 通常会自动创建一个名为 master 的分支来跟踪 origin/master。这正是 git push 和 git pull 一开始就能正常工作的原因。*




