

## 本地

git init 【初始化版本库】

git add 文件名/.    【把文件添加到版本库】

git commit -m '备注'  【将文件提交到仓库】

git status 【查看状态】

git diff 文件名 【查看文件修改前后的不同之处】

git diff HEAD -- 文件名 【查看工作区和版本库某个文件的不同】

git log  --pretty=oneline 单行显示 【查看最近到最远的提交日志】

每次提交都会创建一个版本库

git reset --hard HEAD^ 【回退到上一个版本】也就是指针上移一个版本

git reset --hard HEAD~100 【回退到上一百个版本】

git reset --hard 版本号 【回退到指定版本】 指针指向某个版本库

git reflog 【每次操作记录日志】

目录下新建.gitignore文件可以让版本库忽略某些文件或文件夹

**cat 文件名 【查看某个文件内容】**

git checkout -- 文件名 【把该文件刚才改过的内容撤销】注意：该内容还没有被提交到暂存区

git reset HEAD 文件名 【将添加到暂存区的文件回退到工作区】

**rm 文件名 【删除工作区域的某个文件】**

git checkout -- 文件名 【工作区域删除的文件通过版本库恢复】

git rm 文件名 【直接删除版本库中的某个文件】 再commit 就直接删除了

git add -f 文件名 【强制添加被git忽略的文件】

git check-ignore -v 文件名 【检查git为何不添加该文件】

git config --global alias.st status 【配置别名】

## 远端

git remote add origin 远端url 【本地添加远端仓库】

git push origin 分支名 【本地推送到远端】

git clone 远端url 【克隆一个远端的仓库到本地】

**ls 当前文件夹下文件**

git checkout -b dev_1 【创建dev_1分支并切换到该分支】

git branch 【查看所有分支】

git branch 分支名 【创建一个新的分支】

git merge 分支名 【把某个分支合并到当前分支】

git checkout 分支名 【切换到某个分支】

git branch -d 分支名 【删除某个分支】

git log --graph 【查看版本库线路图】

git merge --no-ff -m '注释' 分支号 【非快速合并会生成一个commit记录】

git stash 【本次工作区写的内容不想加入暂存区想切换分支去干其他事，可以把新加入工作区的内容储存隐藏起来】

git stash list 【查看隐藏存储的节点】

git stash apply 【恢复隐藏存储，但不删除节点】

git stash drop 【删除隐藏存储节点】

git stash pop 【恢复隐藏存储并删除节点】

git stash apply stash@{0} 【恢复某个节点暂存隐藏】

git branch -D 分支号 【某个分支未合并删除会不让删除可以大写D强行删除】

git remote -v 【查看fetch和push的远端分支】

git pull 【获取远端最新的代码】

git rebase 【把所有分支提交合成一条线】

git tag <tagname> 【给该分支最新一次的提交打个标签】

git tag 【查看标签列表】

git tag <tagname> 版本号 【给某次提交打个标签】

git show 标签号 【查看commit详情】

git tag -a <tagname> -m "version 0.1 released" 1094adb  【标签可以备注】

git tag -d <tagname> 【删除某个标签名】

git push origin <tagname> 【将某个标签推送到远端】

git push origin --tags 【将所有标签推送到远端】

git push origin :refs/tags/<tagname> 【删除远端的某个标签】

git log --all --oneline -- pc/src/user/client/page/p2pRecord/p2pRecord.tpl 查找某个删除文件对应的commit信息

#### Fork别人项目到自己的github 然后从自己的账号克隆到本地修改 修改完有推送到自己的远端仓库 推送一个pull request 作者是否接受 看心情



## cmd命令

进入VIM编辑器,可以新建文件也可以修改文件
如果这个文件，以前是没有的，则为新建，则下方有提示为新文件。

按ESC键 跳到命令模式，然后：

:w 保存文件但不退出vi 
:w file 将修改另外保存到file中，不退出vi 
:w! 强制保存，不推出vi 
:wq 保存文件并退出vi 
:wq! 强制保存文件，并退出vi 
q: 不保存文件，退出vi 
:q! 不保存文件，强制退出vi 
:e! 放弃所有修改，从上次保存文件开始再编辑
