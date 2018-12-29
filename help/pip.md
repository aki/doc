###### python2 安装 pip
    
    下载
    wget https://bootstrap.pypa.io/get-pip.py -O get-pip.py
    安装
    python get-pip.py


    设置国内源
    /etc/pip.conf  linux系统
    C:\Users\Administrator\AppData\Roaming\pip\pip.ini  windows系统

    [global]
    index-url = https://pypi.tuna.tsinghua.edu.cn/simple
    
    pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
