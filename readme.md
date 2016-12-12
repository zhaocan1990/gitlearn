#### 初始化本地git仓库(版本库repository)
1、创建空文件夹gitlearn,并进入到文件夹

    $ mkdir gitlearn
    $ cd gitlearn


2、使用`git init`命令将当前文件夹初始化为git仓库

    $ git init
    Initialized empty Git repository in C:/Users/Administrator/Desktop/gitlearn/.git
   文件夹内会生成一个`.git`文件夹，表示仓库创建成功，这个文件夹不能随意修改，不然会破坏仓库

#### 添加文件到仓库
1、创建文件`readme.md`文件
2、使用`git add`命令将文件添加到版本库（仓库）

    $ git add readme.md
   没有提示信息就说明OK
3、使用`git commit`将文件提交到仓库

    $ git commit -m "update"
    [master bb4915f] update
    1 file changed, 12 insertions(+), 9 deletions(-)

`-m "提交说明"` 后面为本次提交的说明
   
4、使用`git status`命令查看当前状态 
       
    $ git status
    On branch master
    Your branch is ahead of 'origin/master' by 1 commit.
      (use "git push" to publish your local commits)
    Changes not staged for commit:
      (use "git add <file>..." to update what will be committed)
      (use "git checkout -- <file>..." to discard changes in working directory)
    
            modified:   readme.md
    
    no changes added to commit (use "git add" and/or "git commit -a")
                    
5、使用`git diff`可以查看修改内容。

     $ git diff readme.md
    diff --git a/readme.md b/readme.md
    index aaa0997..7dd5a98 100644
    --- a/readme.md
    +++ b/readme.md
    @@ -20,9 +20,25 @@

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
