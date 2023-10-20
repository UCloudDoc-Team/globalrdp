# 使用指南

## 如何创建

### 云主机产品入口创建

1.进入云主机产品列表，点击GlobalRDP的“R”灰色图标。不支持GlobalRDP的地域，仍可使用GlobalSSH。
![](/images/globalrdp01.png)

2.选择GlobalRDP的版本

![](/images/globalrdp-create1.png)

3.填写服务器IP、靠近区域、服务器端口等信息，点击确定按钮创建  
![](/images/createglobalrdp-uhost2.png)


### GlobalRDP入口创建

1.进入**网络加速**产品大类下远程桌面加速GlobalRDP入口，点击**创建**按钮  

2.输入需要加速的服务器IP，选择可覆盖你服务器物理位置的区域选项，输入服务器端口号并创建。  
如：假设服务器在洛杉矶，选择洛杉矶选项即可；假设服务器在曼谷，可选择能覆盖曼谷区域的香港或新加坡选项  
![](/images/globalrdp-create.png)


入门版GlobalRDP采用共享IP的方式，不同的实例会分配不同的端口用于RDP连接，因此GlobalRDP端口与服务器端口不一致。

## 如何使用

创建成功后，会生成一个iprdp.net后缀域名。
> 禁止加速域名直接提供HTTP/HTTPS访问。

远程桌面连接，以默认端口3389为例，打开系统RDP客户端，计算机处填写加速域名${AcceleratingDomain}，免费版为${AcceleratingDomain}:${GlobalRDPPort}。输入用户名及密码点击连接，即可。

!> 风险提示：UCloud免费为每个加速IP提供不超过 3 Gbps的基础攻击防御（不同地域支持的最大免费防护流量不同），当加速实例遭受DDoS攻击超过基础防护阈值后，UCloud会对加速区域入口IP采取封堵措施，加速实例将会回源处理。若您的加速实例持续遭受DDoS攻击，产品方保留回收实例权利。
