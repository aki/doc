
```
python2 install pip

wget https://bootstrap.pypa.io/get-pip.py -O get-pip.py
python get-pip.py
```

```
设置国内源

linux     /etc/pip.conf
windows   C:\Users\Administrator\AppData\Roaming\pip\pip.ini

文件内容

[global]
index-url = https://pypi.tuna.tsinghua.edu.cn/simple

命令设置源

pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
```

```
twine upload  
file path: ~/.pypirc

文件内容

[pypi]
repository: https://pypi.org/pypi
username: abc
password: def
