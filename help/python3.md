######  centos7 安装 Python3
    安装tkinter
    yum install tcl tcl-devel tk tk-devel tkinter
    
    安装其它模块
    yum install openssl-devel zlib-devel bzip2-devel sqlite-devel

    安装开发者套件
    yum groupinstall "Development Tools"
    
    下载 python3.6.5
    wget -O Python-3.6.5.tgz http://npm.taobao.org/mirrors/python/3.6.5/Python-3.6.5.tgz
    tar -xzf Python-3.6.5.tgz
    cd ~/Python-3.6.5 
    
    编译安装
    ./configure --prefix=/usr/local/
    make
    make altinstall
    
    链接
    sudo ln -s /usr/local/bin/python3.6 /usr/bin/python3
    sudo ln -s /usr/local/bin/pip3.6 /usr/bin/pip3
