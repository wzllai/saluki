# 概述

saluki是以Grpc作为底层，提供一套高性能、易于使用的分布式远程服务调用(RPC)框架

# 功能

* 与consul配置服务组件进行集成，提供集群环境的服务发现及治理能力。
* 简化开发方式，对于Grpc原生stub方式进行封装，提供了使用interface和pojo作为服务契约的方式
* 与spring-boot进行集成，提供了autoconfig的方式
* 扩展grpc的NameResolver，提供了RoundRobin负载均衡方式

# Quick Start

* 首先使用saluki提供的gradle或插件根据protoc文件生成interface及pojo模型

* 添加spring-boot-saluki依赖

```
     compile group: "com.quancheng.saluki", name: "spring-boot-starter-saluki", version: "1.5.1+"
     compile group: "com.quancheng.saluki", name: "spring-boot-starter-saluki-monitor", version: "1.5.1+"	 
```
