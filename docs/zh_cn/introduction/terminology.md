# 概念说明

- 产品线(Product)
    - 产品线即为BFE中的"租户"。BFE中的配置，比如转发的策略、权限等，是以产品线为单位来进行设置的。

- 集群(Cluster)
    - 具有同类功能的后端的集合定义为一个集群。一个产品线中可定义多个集群。
    - 通常，一个集群的范围可能跨越多个IDC。

- 子集群(Subcluster)
    - 集群又可以划分为多个子集群。
    - 通常，将集群中处于同一IDC中的后端定义为一个子集群。

- 实例(Instance)
    - 每个子集群可包含多个后端服务实例。
    - 对于BFE，每个后端实例表现为"IP地址 + 端口号"。
