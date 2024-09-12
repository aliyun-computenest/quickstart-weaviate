# Weaviate社区版快速部署

## 概述
Weaviate 可以让您快速搭建起公私兼备的网盘系统。Weaviate 在底层支持不同的云存储平台，用户在实际使用时无须关心物理存储方式。你可以使用 Weaviate 搭建个人用网盘、文件分享系统，亦或是针对大小团体的公有云系统。详情请查看[Weaviate官网](https://weaviate.io/developers/weaviate/connections/connect-cloud)。

## 计费说明
Weaviate社区版上的费用主要涉及：

- 所选vCPU与内存规格
- 系统盘类型及容量
- 公网带宽

## RAM账号所需权限
部署Weaviate社区版，需要对部分阿里云资源进行访问和创建操作。因此您的账号需要包含如下资源的权限。
  **说明**：当您的账号是RAM账号时，才需要添加此权限。

| 权限策略名称                          | 备注                                 |
|---------------------------------|------------------------------------|
| AliyunECSFullAccess             | 管理云服务器服务（ECS）的权限                   |
| AliyunVPCFullAccess             | 管理专有网络（VPC）的权限                     |
| AliyunROSFullAccess             | 管理资源编排服务（ROS）的权限                   |
| AliyunComputeNestUserFullAccess | 管理计算巢服务（ComputeNest）的用户侧权限         |

## 部署流程
1. 访问Weaviate社区版服务[部署链接](https://computenest.console.aliyun.com/service/instance/create/cn-hangzhou?type=user&ServiceId=service-c6622482694448288847&ServiceVersion=beta)，按提示填写部署参数：
![image.png](1.jpg)

2. 参数填写完成后可以看到对应询价明细，确认参数后点击**下一步：确认订单**。 确认订单完成后同意服务协议并点击**立即创建**进入部署阶段。

3. 等待部署完成后进入服务实例管理, 在控制台找到Weaviate服务访问链接。
  ![image.png](2.jpg)

4. 单击链接访问服务。参考[文档](https://weaviate.io/developers/weaviate/connections/connect-custom)使用客户端访问服务。
  ![image.png](3.jpg)
  ![image.png](4.jpg)
