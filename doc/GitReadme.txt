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


			
			
			