#### install desktop
    yum groupinstall "GNOME Desktop"
    ln -sf /lib/systemd/system/runlevel5.target /etc/systemd/system/default.target

#### install tab
    yum install bash-completion

#### wubi & set ibus
    yum install ibus-table-wubi im-chooser
    imsettings-switch ibus

#### install ntfs-3g
    wget -O /etc/yum.repos.d/epel.repo http://mirrors.aliyun.com/repo/epel-7.repo
    yum install -y ntfs-3g