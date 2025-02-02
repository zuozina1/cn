# 功能介绍

## 云主机部署位置管理
### 自主控制资源调度及分配
支持指定专有资源池或指定具体专有宿主机创建云主机，若指定专有资源池则系统将按照默认调度规则选择合适的专有宿主机创建。
### 支持多种云主机实例规格类型
对于通用型及内存型专有宿主机，可在其上调度多种实例规格类型，可更加贴近需求灵活地部署业务。
## 资源使用情况监控
###  专有资源池资源使用
支持以专有资源池维度查看池内总CPU、内存、GPU、本地存储等资源使用情况。
### 专有宿主机资源使用
支持指定指定专有宿主机上CPU、内存、GPU、本地存储等资源使用情况。
## 池化分散实现高可用

### 跨可用区
 
创建专有资源池时可指定为多可用区，在池内创建专有宿主机时可由系统在资源池所配置可用区自动选择可用区创建，也可由用户在在资源池所配置可用区范围内指定可用区创建。

### 跨逻辑机架

逻辑机架对应多个物理机架，专有资源池在同一可用区内将提供X个逻辑机架，不同专有宿主机将均衡分散至不同逻辑机架上，通过故障隔离实现高可用。建议进行业务部署时，至少购买两台专有宿主机，避免单点故障。
