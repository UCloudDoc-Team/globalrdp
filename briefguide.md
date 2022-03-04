# 使用指南

## 如何创建

### 云主机产品入口创建

1.进入云主机产品列表，点击GlobalRDP的“R”灰色图标。不支持GlobalRDP的地域，仍可使用GlobalSSH。
![](/images/globalrdp01.png)

2.选择GlobalRDP的版本
![](/images/createglobalrdp.png)

3.填写服务器IP、靠近区域、服务器端口等信息，点击确定按钮创建  
![](/images/grdp02.png)


### PathX入口创建

1.进入PathX产品下的GlobalRDP标签页，点击创建按钮  
![](/images/globalrdp03.png)

2.输入需要加速的服务器IP，选择可覆盖你服务器物理位置的区域选项，输入服务器端口号并创建。  
如：假设服务器在洛杉矶，选择洛杉矶选项即可；假设服务器在曼谷，可选择能覆盖曼谷区域的香港或新加坡选项  
![](/images/grdp02.png)


入门版GlobalRDP采用共享IP的方式，不同的实例会分配不同的端口用于RDP连接，因此GlobalRDP端口与服务器端口不一致。

## 如何使用

成功创建后，会生成一个类似xxx.iprdp.net的域名  
![](/images/gs_20180823151312.png)  

远程桌面连接，以默认端口3389为例，打开系统RDP客户端，计算机处填写加速域名${AcceleratingDomain}，免费版为${AcceleratingDomain}:${GlobalRDPPort}。输入用户名及密码点击连接，即可。
