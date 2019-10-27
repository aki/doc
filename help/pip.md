###### python2 安装 pip
    
    wget https://bootstrap.pypa.io/get-pip.py -O get-pip.py

    python get-pip.py

    设置国内源
    linux     /etc/pip.conf
    windows   C:\Users\Administrator\AppData\Roaming\pip\pip.ini

    [global]
    index-url = https://pypi.tuna.tsinghua.edu.cn/simple
    
    pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
