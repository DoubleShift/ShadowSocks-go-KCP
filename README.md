"# ShadowSocks-go-KCP" 


1. һ��Shadowsocks-go��ű�

��Դ��    ![Shadowsocks-goһ����װ�ű�](https://teddysun.com/392.html)
ϵͳ֧�֣�CentOS��Debian��Ubuntu
�ڴ�Ҫ�󣺡�64M
���ڣ�    2017 �� 02 �� 18 ��

```
chmod +x shadowsocks-go.sh

./shadowsocks-go.sh 2>&1 | tee shadowsocks-go.log

```

2. KCP ����

��Դ��    ![kcptun](https://github.com/xtaci/kcptun)
ϵͳ֧�֣�Debian
�ڴ�Ҫ�󣺡�64M

```
chmod +x server_linux_386

./start.sh

vi /etc/rc.local
���  /root/start.sh

```

�ͻ���������������:
```
client_windows_386.exe -l :4000 -r ������ip:4000 -crypt aes-128 -datashard 10 -parityshard 3 -mtu 1350 -sndwnd 1024 -rcvwnd 1024 -dscp 0 -keepalive 10 -sockbuf 4194304 -mode fast2
```