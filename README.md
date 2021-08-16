# chrony
chrony是网络时间协议（NTP）的通用实现。

chrony包含两个程序：

(1)chronyd是一个可以在启动时启动的守护程序, 用于调整内核中运行的系统时钟和时钟服务器同步。它确定计算机增减时间的比率，并对此进行补偿。

(2)chronyc是一个命令行界面程序，用于监视chronyd的性能并在运行时更改各种操作参数。

关于二者的详细介绍，请参见：https://chrony.tuxfamily.org/documentation.html

# kubenetes下部署chrony服务

## 1、直接kubenetes下yaml文件部署

kubectl apply -f chronyd.yaml

![image](https://user-images.githubusercontent.com/12782056/129527803-9423eaba-4a34-41ce-95f5-f83fb899de34.png)
  
## 2、通过helm部署方

https://artifacthub.io/packages/helm/pnnl-miscscripts/chronyd


# 配置文件解析

这里chrony.conf直接配置的阿里云公网NTP服务器

![image](https://user-images.githubusercontent.com/12782056/129529744-68d4ec72-98b8-4e64-b785-bb08812143a7.png)

![image](https://user-images.githubusercontent.com/12782056/129529356-4e7e18d9-a59a-449f-897e-9aec80d8c878.png)
