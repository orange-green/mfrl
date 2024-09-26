##### 环境配置文档

###### 系统和版本

系统：ubuntu22.03

python版本：3.6 （python3.6不支持vs code debugger）

c依赖：sudo apt-get install libboost-all-dev (没有安装会导致某个c语言头文件报错)

pip 需要安装的tensorflow、magent

tensorflow==1.15 ,用tensorflow2会报错，因为tensorflow2改了api接口属性

magent==0.1.14 

安装g++编译器

```shell
sudo apt update
sudo apt install g++

```

将g++指定为cmake的编译器

```shell
cmake -DCMAKE_CXX_COMPILER=g++ .
```



其余的请按照readme.md文件安装即可

###### 其他注意

ubuntu的源要设置好对应版本的源，不然下载c依赖会下载错误。本机用的阿里云的源，正常可用。

