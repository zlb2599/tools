# Phpstorm安装phpcs

-----

## 第一步：composer引入phpcs
在命令行窗口运行 `composer global require "squizlabs/php_codesniffer=*"`，执行安装即可。


## 第二步：在phpstorm中设置php-cs-fixer

### 菜单
File | Settings | Languages & Frameworks | PHP | Quality Tools

>code sniffer

| 参数              | 参考值                                                       | 备注                                                 |
| :---------------- | :----------------------------------------------------------- | :--------------------------------------------------- |
| PHP code sniffer path               | C:\xxx\phpcs.bat  | phpcs.bat所在路径       |

###  菜单
File | Settings | Editor | Inspections

>php |Quality tools|PHP Code Sniffer vaildation  #选中

>选择 code standard
