## .NET Architecture

.NET阵营需要更多的架构师，我们一起深入.NET应用架构和参考实现。

### 简介
.NET架构从[.NET Architecture Guides](https://dotnet.microsoft.com/learn/dotnet/architecture-guides)开始。

### 容器微服务
根据 .NET framework 确定要面向的操作系统

![containers](https://docs.microsoft.com/zh-cn/dotnet/standard/microservices-architecture/net-core-net-framework-containers/media/image1.png)

### 状态、数据、持久性
在 Docker 中通过 Volume 实现持久化存储和数据共享

![data](https://docs.microsoft.com/zh-cn/dotnet/standard/microservices-architecture/architect-microservice-container-applications/media/image5.png)

基于容器的应用程序的卷和外部数据源

### 分布式数据管理的挑战和解决方案
（一）挑战 1：如何定义每个微服务的边界

定义微服务边界可能是每位用户遇到的第一项挑战，需要标识每个微服务的域模型边界。

（二）挑战 2：如何创建从多个微服务中检索数据的查询
* API 网关
* 使用具有查询/读取表的命令和查询责任分离 (CQRS) 
* 对于可能不需要实时数据的复杂报告和查询，使用数据仓库中的"冷数据"，如Hadoop，它用于不需要实时数据的查询和报告。

（三）挑战 3：如何实现微服务之间的一致性

每个微服务拥有的数据是该微服务专有的，并且只能通过其本身的微服务 API 访问，而不能直接访问其他微服务中的表。

（四）挑战 4：如何设计跨微服务边界的通信

### 微服务的域模型
每个微服务的域模型应该有一个尽可能独立的自治的界定上下文 (Bounded Context, BC)，这样就可以工作而不必不断切换到其他上下文（其他微服务的模型）。
![bc](https://docs.microsoft.com/zh-cn/dotnet/standard/microservices-architecture/architect-microservice-container-applications/media/image10.png)

标识实体和微服务模型边界

### 微服务设计
采用基于菱悦驱动的设计 (DDD) 以及命令和查询责任分离 (CQRS) 方法。

![DDD](https://docs.microsoft.com/zh-cn/dotnet/standard/microservices-architecture/microservice-ddd-cqrs-patterns/media/image6.png)

订单微服务中的 DDD 层

![](https://docs.microsoft.com/zh-cn/dotnet/standard/microservices-architecture/microservice-ddd-cqrs-patterns/media/image11.png)

订单微服务的域模型结构

### API网关
主要功能：
* 身份验证和授权
* 服务发现集成
* 响应缓存
* 重试策略、断路器和 QoS
* 速率限制和遏制
* 负载均衡
* 日志记录、跟踪、相关性
* 标头、查询字符串和声明转换
* IP 允许列表

![Azure API](https://docs.microsoft.com/zh-cn/dotnet/standard/microservices-architecture/architect-microservice-container-applications/media/image14.png)

使用 Azure API 管理 API 网关

### 微服务通信
* 同步： HTTP；
* 异步：AMQP 使用异步消息，如：RabbitMQ。
异步微服务集成强化了微服务的自治性。

![communication](https://docs.microsoft.com/zh-cn/dotnet/standard/microservices-architecture/architect-microservice-container-applications/media/image15.png)

### 微服务（容器）集群
通过多微服务（容器）编排实现伸缩性和高可用性。

![cluster](https://docs.microsoft.com/zh-cn/dotnet/standard/microservices-architecture/architect-microservice-container-applications/media/image28.png)

Azure 容器服务中的群集选项

### 项目
* [eShop](https://github.com/dotnet-architecture/eShopOnContainers)
* [Ocelot](https://github.com/ThreeMammals/Ocelot) 是一个轻型 API 网关

### 书籍
![Microservices & Docker containers](https://dotnet.microsoft.com/images/books/dotnet-microservices-architecture.png)
[下载](https://dotnet.microsoft.com/learn/web/microservices-architecture), [中文版](https://docs.microsoft.com/zh-cn/dotnet/standard/microservices-architecture)

![Modernizing web & server](https://dotnet.microsoft.com/images/books/modernizing-existing-dotnet-applications.png)
[下载](https://dotnet.microsoft.com/learn/web/modernizing-server-apps), [中文版](https://docs.microsoft.com/zh-cn/dotnet/standard/modernize-with-azure-and-containers/)

![ASP.NET apps](https://dotnet.microsoft.com/images/books/architecting-modern-web-applications.png)
[下载](https://dotnet.microsoft.com/learn/web/aspnet-architecture), [中文版](https://docs.microsoft.com/zh-cn/dotnet/standard/modern-web-apps-azure-architecture/)

![Mobile App](https://dotnet.microsoft.com/images/books/enterprise-app-patterns-with-xamarin-forms.png)
[下载](https://dotnet.microsoft.com/learn/mobile/architecture), [中文版](https://docs.microsoft.com/zh-cn/xamarin/xamarin-forms/enterprise-application-patterns/)

![DevOps](https://dotnet.microsoft.com/images/books/containerized-docker-application-lifecycle.png)
[下载](https://dotnet.microsoft.com/learn/web/devops), [中文版](https://docs.microsoft.com/zh-cn/dotnet/standard/containerized-lifecycle-architecture/)

![serverless](https://dotnet.microsoft.com/images/books/serverless-apps-architecture-patterns.png)
[下载](https://dotnet.microsoft.com/learn/cloud/azure-architecture), [中文版](https://docs.microsoft.com/zh-cn/dotnet/standard/serverless-architecture/)

### 图集


### 链接
* [.NET Architecture Guides](https://dotnet.microsoft.com/learn/dotnet/architecture-guides)
* [.NET Application Architecture @ GitHub](https://github.com/dotnet-architecture)
* [官方.NET Docker镜像](https://hub.docker.com/r/microsoft/dotnet/)
