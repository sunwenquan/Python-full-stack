# 1.1 Python开发环境

### CentOS   Python3.6+

源码安装：

```
1. 安装依赖 
2. 下载、解压
3. 进入源码目录，configure
4. make
5. make install 
```

yum 安装

```
yum install python3
# 下面的命令用来解决找不到Python.h
yum list |grep python3 |grep devel
yum install python3-devel.x86_64
```

