1.下载Git客户端和eclipse插件
	
	首先下载 Git客户端，我下载的是 PortableGit-1.7.8
	然后设置环境变量：
		path=.;F:\Program Files\PortableGit-1.7.8\bin
		HOME=%USERPROFILE%
	接着下载EGit,eclipse的插件，插件地址：http://download.eclipse.org/egit/updates
	具体安装过程就不说了
	安装完，进行如下设置：
		Window > Preferences > Team > Git > Configuration
		点击 New Entry ，新建以下键值对：
			github.user     github网站用户名
			github.token    github网站token(登录账户后查看Account Settings)
			user.name		提交的用户名
			user.email		提交时候用的邮箱地址，其实是注册的账户的邮箱地址，可以设置

2.初始化git项目
	按照官网所说，先在github网站上创建 Repositories资源库，例如：HelloGit
	然后会看到项目初始化步骤：
		Global setup:
 			Set up git
  				git config --global user.name "Your Name"
  				git config --global user.email your email
			Add your public key
      	Next steps:
  			mkdir HelloGit
  			cd HelloGit
  			git init
  			touch README
  			git add README
  			git commit -m 'first commit'
  			git remote add origin git@github.com:youraddress/HelloGit.git
  			git push -u origin master
      	Existing Git Repo?
  			cd existing_git_repo
  			git remote add origin git@github.com:youraddress/HelloGit.git
  			git push -u origin master

3.删除不需要的文件夹或文件
	假如你不小心把 bin 目录，或者 classes 目录，更新到了版本库，想删除之，可以这么做：
		git rm -fr bin
		git commit
		git push
		添加 bin 到 .gitignore 文件下（.gitignore应该在当前项目根目录下）
		.gitignore 内容例如：
			/bin
			/.classpath
			/.gitignore

			
			
			