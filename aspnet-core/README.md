## ASP.NET Core
如果基于容器的系统需要实现最佳密度、粒度和性能，.NET Core 和 ASP.NET Core 是最佳选择。 ASP.NET Core 的运行速度比传统 .NET Framework 中的 ASP.NET 高出 10 倍，领先于其他用于微服务的行业技术（例如 Java、Go 和 node.js）。

### 优点
ASP.NET Core 具有如下优点：
* 生成 Web UI 和 Web API 的统一应用场景。
* 针对可测试性进行构建。
* [Razor Pages](https://docs.microsoft.com/zh-cn/aspnet/core/razor-pages/) 可以使基于页面的编码方式更简单高效。
* 能够在 Windows、macOS 和 Linux 上进行开发和运行。
* 开放源代码和[以社区为中心](https://live.asp.net/)。
* 集成[新式客户端框架](https://docs.microsoft.com/zh-cn/aspnet/core/client-side/)和开发工作流。
* 云就绪的[配置系统](https://docs.microsoft.com/zh-cn/aspnet/core/fundamentals/configuration)。
* 内置[依赖注入](https://docs.microsoft.com/zh-cn/aspnet/core/fundamentals/dependency-injection)。
* 轻型的[高性能](https://github.com/aspnet/benchmarks)模块化 HTTP 请求管道。
* 能够在 IIS、Nginx、Apache、Docker 上进行托管或在自己的进程中进行自托管。
* 选择 .NET Core 时，可以使用[并行应用版本控制](https://docs.microsoft.com/zh-cn/dotnet/standard/choosing-core-framework-server)。
* 简化新式 Web 开发的工具。

### Web API 和 Web UI
ASP.NET Core MVC 提供了生成 Web API 和 Web 应用所需的功能：
* [Model-View-Controller (MVC) 模式](https://docs.microsoft.com/zh-cn/aspnet/core/mvc/overview)使 Web API 和 Web 应用可测试。
* Razor Pages 是基于页面的编程模型，它让 Web UI 的生成更加简单高效。
* [Razor 标记](https://docs.microsoft.com/zh-cn/aspnet/core/mvc/views/razor)提供了适用于 Razor 页面和 MVC 视图的高效语法。
* 标记帮助程序使服务器端代码可以在 Razor 文件中参与创建和呈现 HTML 元素。
* 内置的[多数据格式和内容协商](https://docs.microsoft.com/zh-cn/aspnet/core/web-api/advanced/formatting)支持使 Web API 可访问多种客户端，包括浏览器和移动设备。
* [模型绑定](https://docs.microsoft.com/zh-cn/aspnet/core/mvc/models/model-binding)自动将 HTTP 请求中的数据映射到操作方法参数。
* [模型验证](https://docs.microsoft.com/zh-cn/aspnet/core/mvc/models/validation)自动执行客户端和服务器端验证。

### 参考应用 eShopOnWeb
 
git clone https://github.com/dotnet/eShopOnWeb

![eshoponweb](https://docs.microsoft.com/zh-cn/dotnet/standard/modern-web-apps-azure-architecture/media/image2-1.png)

### 体系结构原则
* 分离关注点

在构建应用程序应将核心业务行为与基础结构及用户界面逻辑区分开。
* 封装

正确使用封装有助于在应用程序设计中实现松散耦合及模块化，因为只要维持相同的接口，就可以用不同实现来替代对象和包。

* 依赖关系反转

依赖项反转是生成松散耦合应用程序的关键一环，生成的应用程序的可测试性、模块化程度以及可维护性更高。 遵循依赖关系反转原则可实现依赖关系注入。

* 不要自我重复 (DRY)
* 持久性无感知
* 有界上下文
