# 功能总览

Kubean 主要的功能特性如下：

- 集群全生命周期管理
  - 创建集群，能够应对私有云虚拟化场景，对于物理机将提供 IP 和登录凭证
  - 升级集群，支持 Kubernetes 连续大版本升级，使应用向下兼容
  - 删除集群
  - 一键轮滚证书
  - 详尽的安装/运维日志

- 节点全生命周期管理
  - 通过在线方式和离线方式新增节点
  - 删除节点
  - 节点污点管理
  - 节点标签管理
  - 支持丰富的容器运行时接口（CRI）
    - containerd
    - docker
    - runc
    - docker
    - kata
    - gvisor
- 集群检查：
  - 安装前检查
  - 安装后检查

- 集群组件高可用
  - 单台 master 节点宕机不影响集群正常使用
  - 管理节点故障后，集群运行状态不受影响，业务正常使用
  - 容器管理平台节点故障，可自动弹探测、切换，不影响平台自身的对外提供服务
  