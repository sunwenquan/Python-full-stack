# 1.3.2 创建项目、编写代码

基于技术博客的垂直搜索引擎的项目架构我们已经了解完毕，接下来就是进行项目编码，首先我们得取个名字，我将其命名为：`monkey`。

本次实验的项目目录在 `/home/shiyanlou/Code/monkey` 目录下，实验环境中已经新建该目录，大家可以直接使用。本项目是使用`pipenv`进行包管理。

初始化环境：

```shell
cd ~/Code/monkey
# 执行后会为monkey创建特定的环境，项目根目录会生成Pipfile和Pipfile.lock文件 (实验环境中默认已经安装)
pipenv install
# 安装pip==18.0 (实验环境中默认已经安装)
pipenv run pip install pip==18.0
# 创建代码目录
mkdir monkey
# 创建说明文档目录
mkdir docs
# 创建测试文件夹
mkdir tests
# 创建README.md
touch README.md
```



目前，最外一层项目目录结构如下：

```shell
.
├── Pipfile
├── Pipfile.lock
├── README.md
├── docs
├── monkey
└── tests
```



此时，项目的基本环境已经搭建完毕，利用 pipenv 可以很方便地对包以及项目环境进行管理：

```shell
# 进入项目 monkey 的虚拟环境，在 monkey 虚拟环境中默认使用的就是 Python3.6
pipenv shell
看到以下类似的输出即可理解为项目环境搭建成功：
```