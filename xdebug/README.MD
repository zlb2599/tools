## php.ini
xdebug.idekey=PHPSTORM
xdebug.remote_host=host.docker.internal
xdebug.remote_port=9001
xdebug.remote_enable=1 
##phptorm
1.菜单:File | Settings | Languages & Frameworks | PHP | Debug

> debug port:9001 # 与xdebug.remote_port一致

2.菜单:File | Settings | Languages & Frameworks | PHP | Debug | DBGp Proxy

> IDE key:PHPSTORM #与xdebug.idekey一致
> host:local.project #虚拟主机
> port:80 #网站端口

3.菜单:File | Settings | Languages & Frameworks | PHP | Servers
添加
> name :project  #随便起
> host :local.project #虚拟主机
> port:80 #网站端口
> Debuger :xdebug
> use path mapping :  #选中
> File/directory:  #项目本地路径
> absolute path on the server # docker 对应目录

4.编辑器右上角 add configureation  (run/debug configureation)
添加 php web page
> server # 选择第三步新建的server


