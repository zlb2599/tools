
# Phpstorm安装xdebug及使用方法

-----

##  配置php.ini

xdebug.idekey=PHPSTORM
xdebug.remote_host=host.docker.internal #PHPSTORM所在机器IP
xdebug.remote_port=9001 #xdebug 监听端口
xdebug.remote_enable=1 

## 配置phptorm

### 1.菜单:File | Settings | Languages & Frameworks | PHP | Debug

>debug port:9001 # 与xdebug.remote_port一致

### 2.菜单:File | Settings | Languages & Frameworks | PHP | Debug | DBGp Proxy

| 参数              | 参考值                                                       | 备注                                                 |
| :---------------- | :----------------------------------------------------------- | :--------------------------------------------------- |
| IDE key              | PHPSTORM                                                 | 与xdebug.idekey一致                                             |
| host       | local.project                                                     | 虚拟主机                                   |
| port           | 80                                     | 网站端口   |

### 3.菜单:File | Settings | Languages & Frameworks | PHP | Servers
添加

| 参数              | 参考值                                                       | 备注                                                 |
| :---------------- | :----------------------------------------------------------- | :--------------------------------------------------- |
| NAME              | project                                                 | 任意填写                                             |
| host       | local.project                                                     | 虚拟主机                                   |
| port           | 80                                     | 网站端口   |
| Debuger         | xdebug |  |
| use path mapping | 选中                                             |                        |
| File/directory | D:/docker/www/project                                              |         项目本地路径               |
| absolute path on the server | /var/www/html/project                                            |         docker 对应目录               |

4.编辑器右上角 add configureation  (run/debug configureation)
添加 php web page
> server # 选择第三步新建的server

