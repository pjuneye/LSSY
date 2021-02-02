# LSSY量化交易系统

支持A股和可转债市场并且可以实盘全自动交易的量化交易系统。

开源的目的是希望能有更多的人来参与社区维护，共同打造最完美的量化交易系统。

目前市场上集量化回测、实盘交易的系统并不多，适用A股的更是寥寥无几，要么收费高昂，LSSY量化交易系统为了让研究量化交易的朋友人人都能用，所以在此开源，并且完全免费，希望更多的人来参与完善系统，贡献自己的一份力量。

LSSY量化交易系统致力于量化交易，不再主观交易，通过数据，做大概率，让量化交易变得更容易，大家都可以参与完善，**为了更好的利于社区发展，目前采用邀请制，使用邀请码才能完整的使用LSSY量化交易系统**，提交代码或者邀请朋友都可以免费获得邀请码（在社区讨论QQ群发放）。我们是希望大家互相告知让更多的宽客去实现自己的策略梦想，避免重复造轮子。

# 安装

  * **Windows**
  
    1.安装Linux子系统，选择ubuntu子系统。
    
    2.给子系统安装pip3
    
    ```
    sudo apt install python3-pip
    ```
    
    3.安装数据库
    
    ```
    sudo apt install redis
    ```
    
    4.启动数据库，子系统不能自动启动，所以每次都需要手动启动数据库服务，所以不建议在Windows上运行。
    
    ```
    redis-server
    ```
    
    Windows安装视频教程：https://www.bilibili.com/video/BV1pi4y1c7ZR
  
  * **Linux**
  
    1.安装 redis 数据库
    
    ```
    sudo apt install redis
    ```

    2.需要 python3.8
    
    下载源码编译安装：https://www.python.org/ftp/python/3.8.7/Python-3.8.7.tar.xz

 * **Mac OS**
 前提是先安装 brew 
 1. 安装 redis 数据库
  ```
    brew install redis
    ```
 2. 安装Python 3.8 (建议使用pyenv) 
 ```
    brew install pyenv
    ```
     ```
   pyenv install 3.8.7
    ```
   

# 执行安装脚本

```
./install.sh
```

# 启动LSSY量化交易系统

进入实盘交易

```
./runWork.py
```

进入回测

```
./runWork.py b
```

# 访问前端

推荐分辨率>=2k

```
http://127.0.0.1:8000/
```

# 初次启动注意事项

首次部署LSSY量化交易系统，会下载大量财务历史等数据，根据网络情况可能会很慢，建议晚上睡觉前启动系统，一般到第二天就全部下载完成了，仅首次运行，后续每天只需要更新k线即可，速度会快很多。

QQ群讨论社区：174647513





