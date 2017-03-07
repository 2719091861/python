# python
<<<<<<< HEAD

# python
https://git-scm.com/book/en/v2/Getting-Started-Getting-Help//git设置
git add . #将文件加入stage area
git commit #提交文件，同时提示输入commit message
git push -u origin master #push到远程仓库，同时设置跟踪分支，下次push的时候，直接输入git push就醒了，系统会自动用本地master分支跟踪远程master分支
ssh -T git@github.com
echo "# learn-app" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:2719091861/learn-app.git
git push -u origin master

git remote add origin git@github.com:2719091861/learn-app.git
git push -u origin master
git clone git@github.com:2719091861/learn-app.git

【第二步】克隆仓库

　　第二步开始就基本进入命令行模式了，不过要先从github上下载命令行工具。下载地址：http://windows.github.com/ 

　　然后进行简单的安装之后，会在桌面上创建两个图标，GitHub和Git Shell，GitHub是图形界面，Git Shell是命令行模式，而且默认的Git仓库是建在C盘的，个人建议要把路径重设下。

　　点开Git Shell，进入命令行。首先我们先要把GitHub上的我们新建的仓库clone下来，为了演示，我在GitHub上新建了一个名称为myRepoForBlog的git。

　　在初始化版本库之前，先要确认认证的公钥是否正确，如下：

　　ssh -T git@github.com

　　正确地结果如下：　

　　Warning: Permanently added 'github.com,207.97.227.239' (RSA) to the list of known hosts.
　　Hi findingsea! You've successfully authenticated, but GitHub does not provide shell access.

　　会有一个Warning，不用理会。

　　接下对库进行clone，如下：

　　git clone https://github.com/findingsea/myRepoForBlog.git

　　上面的地址可以在如下界面找到：

　　

　　clone成功如下：

　　Cloning into 'myRepoForBlog'...
　　Warning: Permanently added 'github.com,207.97.227.239' (RSA) to the list of known hosts.
　　remote: Counting objects: 3, done.
　　remote: Total 3 (delta 0), reused 0 (delta 0)
　　Receiving objects: 100% (3/3), done.

　　【第三步】上传README.md文件

　　这个时候，我们的GitHub文件夹下就多了一个myRepoForBlog文件夹，进入文件夹目录，对仓库进行初始化，如果我们之前没有勾选创建README，则要先创建README.md文件，不然上传文件会报错。如果在第一步就勾选过了，则可以直接进入第四步。

　　git init
　　touch README.md
　　git add README.md
　　git commit -m 'first_commit'
　　git remote add origin https://github.com/findingsea/myRepoForBlog.git
　　git push origin master

　　【第四步】push文件

　　创建完README.md后，就可以push了，代码类似。

　　git add .
　　git commit -m 'first_commit'
　　git remote add origin https://github.com/findingsea/myRepoForBlog.git
　　git push origin master

　　如果执行git remote add origin https://github.com/findingsea/myRepoForBlog.git，出现错误：

　　fatal: remote origin already exists

　　则执行以下语句：

　　git remote rm origin

　　再往后执行git remote add origin https://github.com/findingsea/myRepoForBlog.git 即可。

　　在执行git push origin master时，报错：

　　error:failed to push som refs to.......

 

　　则执行以下语句：

　　git pull origin master

　　先把远程服务器github上面的文件拉先来，再push 上去。

 　　【结束】

　　再次要强调这篇文章主要是对初学者的，也就我这种github菜鸟的。

　　最后感谢那些无私分享自己经验和知识的博主们。

=======
>>>>>>> 6a0380f708cc831124cb878a5df01e051215aa47
