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

cat 文件名 【查看某个文件内容】

git checkout -- 文件名 【把该文件刚才改过的内容撤销】注意：该内容还没有被提交到暂存区

git reset HEAD 文件名 【将添加到暂存区的文件回退到工作区】

rm 文件名 【删除工作区域的某个文件】

git checkout -- 文件名 【工作区域删除的文件通过版本库恢复】

git rm 文件名 【直接删除版本库中的某个文件】 再commit 就直接删除了


远端

git remote add origin 远端url 【本地添加远端仓库】

git push origin 分支名 【本地推送到远端】














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