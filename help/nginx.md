#### install nginx
    安装PCRE库（Nginx的rewrite模块和HTTP核心模块会用到PCRE正则表达式语法）
    yum install pcre pcre-devel

    安装OpenSSL（若服务器提供安全网页(https://)时，会用到OpenSSL库）
    yum install openssl openssl-devel
    
    gzip 类库安装
    yum install zlib zlib-devel
    
    下载地址： http://nginx.org/download/
    tar -xzf nnginx-1.9.9.tar.gz
    cd nginx-1.9.9/
    
    开启ssl 模块 启用“server+status"页
    ./configure --with-http_stub_status_module --with-http_ssl_module
    
    make
    make instatll

    开放80端口
    /sbin/iptables -I INPUT -p tcp --dport 80 -j ACCEPT
    
    nginx 停止命令
    /usr/local/nginx/sbin/nginx -s stop
    nginx 重载配置
    /usr/local/nginx/sbin/nginx -s reload
