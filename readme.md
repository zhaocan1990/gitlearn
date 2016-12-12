##### 初始化本地git仓库(版本库repository)
1、创建空文件夹gitlearn,并进入到文件夹     

    $ mkdir gitlearn     

    
2、使用`git init`命令将当前文件夹初始化为git仓库 

  `$ git init`    
  `Initialized empty Git repository in C:/Users/Administrator/Desktop/gitlearn/.git`  

   文件夹内会生成一个`.git`文件夹，表示仓库创建成功，这个文件夹不能随意修改，不然会破坏仓库

##### 添加文件到仓库
1、创建文件`gitlearn.md`文件  
2、使用`git add`命令将文件添加到版本库（仓库）  

    $ git add gitlearn
    
3、使用`git commit`将文件提交到仓库

*  要随时掌握工作区的状态，使用`git status`命令。

*  如果git status告诉你有文件被修改过，用`git diff`可以查看修改内容。
*
*  查看分支：git branch
*
*  创建分支：git branch <name>
*
*  切换分支：git checkout <name>
*
*  创建+切换分支：git checkout -b <name>
*
*  合并某分支到当前分支：git merge <name>
*
*  删除分支：git branch -d <name>
