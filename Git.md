Git:版本管理软件  Github:存放Git管理的项目

1）git基本操作

​		git init：把文件夹变成一个git仓库

​		git status：当前文件的情况

​		git add . ：把一个没有追踪的修改给追踪了 这个时候再查看git status的时候就发现更改准备提交了

​		然后进入这个文件做一些修改 再查看git status的时候 就发现没有被提交 所以当你做了修改以后还需要再添加一次 才能提交

​		git diff：就可以查看修改了的这次与之前的不同 现实出来这次还没有被添加的修改 其修改的内容是什么 然后执行git add 把修改的内容给添加上去 这个时候查看git status就会发现没有modified file了

​		git reset：撤回添加 就没有被追踪了

​		git config --global user.name "Swag"   ：提交之前 告诉git你是谁

​		git config --global user.email "15319086647@163 . com"   ：提交之前 告诉git你的邮箱

​		git commit -m "提交的描述"  ：提交更改

​		git commit ：打开默认编辑器然后添加提交的描述

​		新建一个.gitignore文件 在这个文件里写上你想忽略的文件：只是不想让git管理这一个文件

​		git rm --cached newfile ：只要你让git追踪一个文件 那么git就会一直追踪这个文件 除非你让git停止追踪这个文件

 2）git分支

​		想大幅度修改代码

​		git branch 分支的名字：添加一个git分支

​		git checkout 分支名称：切换git分支 然后在你新建的git分支里面乱改 

​		git checkout master：切换到主分支 文件夹里也会跟着改变

​		git merge pictures：在主分支下 把pictures分支合并起来 文件夹里也会跟着改变 然后这个时候输入git branch发现还是有两个分支 采用git branch -d pictures 会把pictures分支删掉 -D是你还没有merge的时候 强制删掉当前的分支

3）github

​		git remote add origin 文件网址：把本地文件与github上进行链接

​		git push --set-upstream origin master：将本地文件传入github

​		git config credential.helper store：输入完密码后再也不用输入密码

​		git remote rm origin：删除关联的远程仓库

​		git pull 把项目最新的状态拉到本地



​		 git remote set-url origin https://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@github.com/SwaaggyP/learnGit.git

​		git token: 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