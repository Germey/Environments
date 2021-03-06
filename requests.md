# requests 的安装

由于 requests 属于 Python 第三方库，也就是 Python 默认不会自带这个库，需要我们手动去安装，下面我们首先看一下它的安装过程。

## 相关链接

* GitHub：[https://github.com/requests/requests](https://github.com/requests/requests)
* PyPy：[https://pypi.python.org/pypi/requests](https://pypi.python.org/pypi/requests)
* 官方文档：[http://www.python-requests.org](http://www.python-requests.org)
* 中文文档：[http://docs.python-requests.org/zh_CN/latest](http://docs.python-requests.org/zh_CN/latest)

## 安装方法

### pip 安装

无论是 Windows、Linux 还是 Mac，都可以通过 pip 这个包管理工具来安装。

在命令行下运行如下命令即可完成 requests 库的安装：

```
pip3 install requests
```

这是最简单的安装方式，推荐此种方法安装。

### wheel 安装

wheel 是 Python 的一种安装包，其后缀为 whl，在网速较差的情况下可以选择下载下 wheel 文件再安装，直接用 pip3 命令加文件名安装即可。

不过在这之前需要先安装 wheel 库，安装命令如下：

```
pip3 install wheel
```

然后到 PyPi 上下载对应的 wheel 文件，如当前最新版本为 2.17.3，则打开：[https://pypi.python.org/pypi/requests/2.17.3#downloads](https://pypi.python.org/pypi/requests/2.17.3#downloads)，下载 requests-2.17.3-py2.py3-none-any.whl 到本地。

随后命令行进入 Wheel 文件目录，利用 pip 安装即可。

```
pip3 install requests-2.17.3-py2.py3-none-any.whl 
```

这样我们同样可以完成 requests 的安装。

### 源码安装

那么如果你不想用 pip 来安装，或者想获取某一特定版本，可以选择下载源码安装。

此种方式需要先找到此库的源码地址，然后下载下来再用命令安装。

requests 项目的地址是：[https://github.com/kennethreitz/requests](https://github.com/kennethreitz/requests)。

可以通过 Git 来下载源代码：

```
git clone git://github.com/kennethreitz/requests.git
```

或通过 curl 下载：

```
curl -OL https://github.com/kennethreitz/requests/tarball/master
```

下载下来之后，进入目录，执行如下命令安装即可：

```
cd requests
python3 setup.py install
```

命令执行结束后即可完成 requests 的安装，由于此种安装方式比较繁琐，后文此种安装方式不再赘述。

## 验证安装

为了验证库是否已经安装成功，可以在命令行下测试一下：

```
$ python3
>>> import requests
```

在命令行首先输入 python3，进入命令行模式，然后输入如上内容，如果什么错误提示也没有，那么就证明我们已经成功安装了 requests。