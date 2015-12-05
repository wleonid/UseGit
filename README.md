# UseGit
学习使用Git之路


学习途径：学习廖雪峰的Git教程

学习步骤：

		  1.配置全局user.name和useremail
		  		$git config --global user.name ""
		  		$git config --global user.email ""
		  2.初始化Git仓库，使用git init命令
		  	添加文件到仓库，使用git add和git commit -m
		  3.用git status掌握仓库目前状态
		    用git diff查看文件具体修改内容，在git add前
		  4.git log 查看从最近到最远的提交日志
		  	git log --pretty=oneline 提交日志只显示commit id（版本号）和版本描述
		  	HEAD表示当前版本
		  	HEAD^表示上一版本
		  	HEAD^^表示上上一个版本
		  	HEAD~100表示上100个版本
		  	git reset --hard HEAD^ 回退到上一版本
		  	git reset --hard 版本id前几位 回到此id的版本
			git reflog 记录每次的命令
		  5.工作区、暂存区
		  	工作区的修改通过git add添加进暂存区
		  	暂存区的文件通过git commit进行提交
		  	git diff HEAD -- 文件名 查看工作区和版本库中最新版本的区别
		  6.git checkout --文件名 让文件回到最近一次commit或add时的状态
		  	git reset HEAD 文件名 撤销add,即回到最新的版本
		  	当改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用git checkout --
		  	当不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，首先git reset HEAD file,就回到了前一个场景，第二步按之前场景的做法做
		  7.git rm 文件名 删除版本库中的文件
		  8.$ ssh-keygen -t rsa -C "youremail@example.com"
		  	把id-rsa.pub（C盘用户administrative/ssh文件夹）的内容复制到网站添加ssh的位置
		  	$git remote add origin 添加远程库
		  	$git push -u origin master 
		  	$git push origin master
		  	$git clone
		  9.创建并切换到dev分支：$git checkout -b dev
		  	创建分支不切换:$git branch 分支
		  	切换分支：$git checkout 分支名
		  	查看分支：$git branch    （带*的表示当前分支）
		  	合并指定分支到当前分支 $git merge 分支名
		  	删除分支：$git branch -d 分支名





