##基于grunt自动化开发工具的微信official website解决方案 

开发人员根据项目的实际情况进行扩展；	

###如何操作，请按下步骤进行；	

####克隆笨仓库
在开发目录下执行：

````
git clone https://github.com/FEsy/wsite.git
````
####安装Npm依赖包

详细的依赖包清单请参考`package.json`文件，Grunt相关配置请看`Gruntfile.js`

````
npm install
````

安装完毕之后，你将得到如下的文件结构

####文件目录结构
后续在做补充
````
````


####初始化

git clone下来后，可以将`StaticPage`文件夹修改成项目的文件名，建议初始化时可执行一次:

````
grunt bundle
````

####Grunt配置

######CSS编译&&压缩

对于`Sass`可自动编译和纠错，使用`cssmin`对文件进行压缩，可有效减少文件大小.

使用

````
grunt sass
````

可进行Sass编译。若直接使用原生css，可直接执行`grunt`。

######JS文件

使用`concat`根据自己的需求对js进行压缩（对多个文件压缩时需要进行配置），默认使用`uglify`对js文件进行压缩，在最终的min.v.js文件前面加上时间戳（可以根据需求删除）。

######文件监听

使用

````
grunt watch
````
可监听所有的开发目录下`.scss`,`.css`,'.js'的变化，自动编译压缩。

可以单独使用`grunt watch:base`进行普通监听`js`目录下所有文件和`css/style.css`。

使用`grunt watch:sass`或者`grunt watch:css`分别监听`.scss`和`.css`文件。



更多配置参考官网api [grunt](http://gruntjs.cn/configuring-tasks/)

###说明
####plugins:		

####components:	

上面两个文件作为我们团队的重点维护对象，后续将以库的形式存在	
此解决方案为微信site v1.0解决方案后续将会在此基础上升级；

###后续更新	

本团队开发人员可以新建一个分支，新的分支上进行扩展，最后合并到主分支；


###申明
本文参考了		

[适合简单静态页面的grunt自动化开发工具](https://github.com/foru17/StaticPage)		

[开发seajs项目的超级利器](https://github.com/fouber/spmx)	

###版本更新说明