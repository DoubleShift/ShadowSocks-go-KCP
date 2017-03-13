"# ShadowSocks-go-KCP" 


1. 一键Shadowsocks-go搭建脚本

来源：    ![Shadowsocks-go一键安装脚本](https://teddysun.com/392.html)
系统支持：CentOS，Debian，Ubuntu
内存要求：≥64M
日期：    2017 年 02 月 18 日

```
chmod +x shadowsocks-go.sh

./shadowsocks-go.sh 2>&1 | tee shadowsocks-go.log

```

2. KCP 配置

来源：    ![kcptun](https://github.com/xtaci/kcptun)
系统支持：Debian
内存要求：≥64M

```
chmod +x server_linux_386

./start.sh

vi /etc/rc.local
添加  /root/start.sh

```

客户端配置命令如下:
```
client_windows_386.exe -l :4000 -r 服务器ip:4000 -crypt aes-128 -datashard 10 -parityshard 3 -mtu 1350 -sndwnd 1024 -rcvwnd 1024 -dscp 0 -keepalive 10 -sockbuf 4194304 -mode fast2
```