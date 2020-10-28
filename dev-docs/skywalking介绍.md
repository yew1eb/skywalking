## SkyWalking是什么？
SkyWalking: 一个开源的可观测平台, 用于从服务和云原生基础设施收集, 分析, 聚合及可视化数据。
SkyWalking 提供了一种简便的方式来清晰地观测分布式系统, 甚至横跨多个云平台。
SkyWalking 更是一个现代化的应用程序性能监控(Application Performance Monitoring)系统, 尤其专为云原生、基于容器的分布式系统设计.

## 架构
SkyWalking 逻辑上分为四部分: 探针, 平台后端, 存储和用户界面.
![](http://skywalking.apache.org/assets/frame-v8.jpg?u=20200423)

+ 探针 基于不同的来源可能是不一样的, 但作用都是收集数据, 将数据格式化为 SkyWalking 适用的格式.
+ 平台后端, 支持数据聚合, 数据分析以及驱动数据流从探针到用户界面的流程。分析包括 Skywalking 原生追踪和性能指标以及第三方来源，包括 Istio 及 Envoy telemetry , Zipkin 追踪格式化等。 你甚至可以使用 Observability Analysis Language 对原生度量指标 和 用于扩展度量的计量系统 自定义聚合分析。
+ 存储 通过开放的插件话的接口存放 SkyWalking 数据. 你可以选择一个既有的存储系统, 如 ElasticSearch, H2 或 MySQL 集群(Sharding-Sphere 管理),也可以选择自己实现一个存储系统. 当然, 我们非常欢迎你贡献新的存储系统实现。
+ UI 一个基于接口高度定制化的Web系统，用户可以可视化查看和管理 SkyWalking 数据。

## 部署模块
![](http://skywalking.apache.org/doc-graph/communication-net.png)


