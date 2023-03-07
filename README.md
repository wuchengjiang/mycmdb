# 资产管理系统CMDB和DNS管理系统



## 主要功能

用户增删改查和权限管理、服务器资产的收集和管理、智能DNS的配置和管理、服务树的管理
   
## 开发语言

 服务端 golang 、beego框架; 客户端 python 2.7 
   

## 架构设计

1. 平台采用C/S 架构
2. 服务端beegoAdmin开发REST API 接口和UI; 客户端 IDC机房kvm资产通过ansible采集资产信息，云上主机通过云厂商提供的sdk定时采集信息，调用服务端提供的rest接口上报到服务端
3. 平台管理界面对项目、应用、项目负责人、资产等信息进行管理
4. 智能DNS管理平台后端技术采用bind-dlz，前端UI对DNS进行配置和管理


## 系统展示

**主机管理**
![](https://raw.githubusercontent.com/wuchengjiang/mycmdb/main/images/%20%E4%B8%BB%E6%9C%BA%E7%AE%A1%E7%90%86.png)

**资产管理**
![](https://raw.githubusercontent.com/wuchengjiang/mycmdb/main/images/zichanguanli.png)

**服务树**
![](https://raw.githubusercontent.com/wuchengjiang/mycmdb/main/images/servicetree.png)

**智能DNS**
![](https://raw.githubusercontent.com/wuchengjiang/mycmdb/main/images/%E6%99%BA%E8%83%BDdns%E7%B3%BB%E7%BB%9F.png)