## 专业术语

|   **英文**    |   **中文**   | **说明**                                                     |
| :----------- | :---------- | ----------------------------------------------------------- |
|      VPC      |   虚拟网络   | 合作私有网络（Cloud on Cloud Virtual Private Cloud，简称CoCVPC），是京东云与合作伙伴云厂商合作推出的云上自定义的逻辑隔离的网络空间，以下简称私有网络（VPC）。与您在数据中心搭建的传统网络类似，此私有网络空间由用户完全掌控，支持自定义网段划分、路由策略等。用户可以在VPC内创建和管理合作云产品，如合作云主机，同时可配置网络内的资源连接Internet。 |
|    Subnet     |     子网     | 子网是所属VPC IP地址范围内的 IP 地址块。目前私有网络中的部分云资源部署在子网内，如云主机。子网base在VPC下，在创建 VPC后，您可以在VPC下添加子网。相同VPC下子网的IP地址块不可以重叠，不同VPC下子网的IP地址块可以重叠。 |
|      Route Table      |    路由表    | 路由表是一系列路由规则的集合，用于控制私有网络中子网的流量流出方向。京东云共有两种类型的路由表：默认路由表和自定义路由表。随私有网络创建时自动创建的路由表为默认路由表，用户主动创建的路由表为自定义路由表。每个子网都必须关联一张路由表且只能关联一张路由表，每张路由表可以关联多个子网。 |
|      ACL      | 访问控制列表 | 子网级别无状态的可选安全层，用于控制进出子网的数据流，可以精确到协议和端口粒度，可用作防火墙来控制进出一个或多个子网的流量。没有网络ACL的保护或者没有配置访问控制策略，会导致子网中的服务器所有网络端口更容易在互联网上遭受攻击甚至导致被入侵。网络ACL可用于对跨子网的东西向访问流量或者进出互联网的南北向访问流量进行过滤。具有相同网络流量控制的子网可以关联同一个网络 ACL，通过设置出站和入站允许规则，对进出子网的流量进行精确控制。 |
|  Elastic IP   |  弹性公网IP  | 弹性公网IP是可以独立申请的公网IP地址，支持与云主机、负载均衡、NFV实例等资源进行动态绑定和解绑，弹性公网IP支持两种类型：标准公网IP和边缘公网IP。 |
|      BGP      | 边界网关协议 | BGP为Border Gateway Protocol的缩写。网络运营商之间通过BGP协议互相宣告IP地址段，BGP IP可以实现单IP多线路，达到不同运营商用户可以高速访问的效果。 |
|    Region     |     地域     | 不同的地域即不同的地理区域。目前京东云有四个地域，分别为华北-北京、华南-广州、华东-宿迁、华东-上海。 |
| Availability Zone |    可用区    | Availability Zone简称AZ。单个地域下可以包含多个AZ，不同AZ之间实现资源隔离，保障资源的高可用性。同地域下的AZ通常采用低延迟与高带宽的线路进行互联。AZ代表是中心可用区。 |
|   Instance    |     实例     | 特指云主机等资源。                                       |

## 相关参考
- [VPC](Features/VPC-Features.md)
- [产品优势](Benefits.md)
- [创建VPC](../Operation-Guide/VPC-Configuration.md)
- [地域及可用区](Region-Az.md)
