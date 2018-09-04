###### 国内访问 github.com 速度慢的解决方法
    ipaddress地址：https://www.ipaddress.com

    主要修改的hosts地址为：github.com 和 github.global.ssl.fastly.net

    windows Hosts 文件 C:\Windows\System32\drivers\etc\hosts
    linux Hosts 文件  /etc/hosts
 
    linux刷新DNS缓存: sudo /etc/init.d/networking restart
    windows刷新DNS的方法：ipconfig /flushdns
    
    192.30.253.112     github.com	
    192.30.253.113     github.com
    151.101.185.194    github.global.ssl.fastly.net