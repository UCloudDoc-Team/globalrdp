# FAQ

## GlobalRDP最大空闲连接时间  
通常是300s（少部分转发机器会限制在90s），如果需要保持长连接，请在客户端或服务端开启keepalive保活并减少探测间隔时间。

## 如何使用 GlobalRDP 白名单功能？
暂不支持白名单功能。

## 使用 GlobalRDP 端口不通  
1）实例运行需要1分钟的启动时间。超出该时间后，先确认源站的相同端口是否可以连接；

2）中国大陆地区Ping GlobalRDP 的域名，如果可以 Ping 通，试试 telnet GlobalRDP域名 端口 是否可以连接（无法连接提供给我们）；如果 Ping 不通，请dig下 GlobalRDP域名，将结果提供给我们。
