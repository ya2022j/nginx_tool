## ###   使用docker安装redmine部署成功

##　2023.03.19　リリース

* 1. 在docker-compose.yaml中增加了privileged:true的内容，解决了docker容器 "restarting..."，其实是权限不足的问题
* 2. 使用nginx去部署docker容器的时候，在server的模块中不要增加静态文件的路径指定，就原封不动的使用docker容器的默认路径即可，不然问题非常多。昨天就是上传文件失效，弄了很久。后面凡是用docker来安装的应用，用到nginx去代理的时候，不要在server里面设置静态路径。直接使用应用的默认的路径即可
* 3. 还有一个windows的安装包。资源如下，但是默认的账户和密码有些问题。暂时用不到。先收着即可。

bitnami-redmine-5.0.0-1-windows-x64-installer.exe_免费高速下载|百度网盘-分享无限制 https://pan.baidu.com/s/1vTu-PdUaPFd9ek9UYN998A 提取码：ning
