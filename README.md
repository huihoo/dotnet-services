# .NET Services
![.NET](https://wiki.huihoo.com/images/f/f2/Microsoft.NET.png)

我们一起设计和完善.NET平台（C#,F#和Q#语言）咨询、培训、教育课程。

### 本课程的初衷和目标
.NET(C#,F#)是自由、开放的开发者平台和编程语言，我们一起交流、学习、掌握.NET(C#和F#)。相信很多朋友都会有这样的体会：C#比Java设计实现的更好，对开发者很友好，生产力更高。因为现在就业市场大多都是Java，而C#的需求有些少，所以是该有所改变的时候了。

### 基金会
通过[.NET Foundation](https://github.com/dotnet)进行社区治理，而非一家公司。

### 生态系统
[重建中国.NET生态系统](https://www.cnblogs.com/neuzilla/p/recreate-dotnet-ecosystem-neuzilla.html) .NET阵营的情况是紧缺资深架构师，这个问题不解决，再牛的语言也是白搭。Java自从被Oracle收购后总存在一些治理问题，C#和.NET生态机会很大。

![awesome](https://wiki.huihoo.com/images/1/13/Awesome.png)
* [Awesome .NET](https://github.com/quozd/awesome-dotnet) 
* [Awesome .NET Core](https://github.com/thangchung/awesome-dotnet-core/) 
* [Awesome F#](https://github.com/fsprojects/awesome-fsharp) 
* [Awesome Xamarin](https://github.com/benoitjadinon/awesome-xamarin) 
* [Awesome Umbraco](https://github.com/leekelleher/awesome-umbraco) 

### .NET
一个自由、跨平台、开源的开发者平台，帮助你构建所有的应用：web、mobile、desktop、gaming、IoT

[.NET中文文档](https://github.com/dotnet/docs.zh-cn/blob/live/docs/welcome.md)

### .NET Core
.NET Core 是一个通用目的、模块化、跨平台的 .NET 开源实现。

.NET Core 是.NET Framework的新一代版本，具有跨平台 (Windows、OS X、Linux) 能力的应用程序开发框架 (Application Framework)，未来也将会支持 FreeBSD 与 Alpine 平台，也是微软在一开始发展时就开源的软件平台。

由于 .NET Core 的开发目标是跨平台的 .NET 平台，因此 .NET Core 会包含 .NET Framework 的类库，但与 .NET Framework 不同的是 .NET Core 采用包 (Packages) 的管理方式，应用程序只需要获取需要的组件即可，与 .NET Framework 大包式安装的作法截然不同，同时各包也有独立的版本线 (Version line)，不再硬性要求应用程序跟随主线版本。

[.NET Core入门](https://github.com/dotnet/docs.zh-cn/blob/live/docs/core/get-started.md)

### ASP.NET
ASP.NET是由微软在.NET Framework框架中所提供，开发Web应用程序的类库，封装在System.Web.dll文件中，使用System.Web命名空间。

[ASP.NET文档](https://github.com/aspnet/Docs.zh-cn/blob/live/aspnet/index.md)

### ASP.NET Core
ASP.NET Core 可运行于 Windows 平台以及非 Windows 平台，如 macOS 以及 Linux 操作系统，是 Microsoft 第一个具有跨平台能力的 Web 开发框架。

采用 Apache v2 许可协议，由 .NET 基金会 (.NET Foundation) 管理。

[ASP.NET Core文档](https://github.com/aspnet/Docs.zh-cn/blob/live/aspnetcore/index.md)

### PowerShell
Windows PowerShell 是微软为Windows环境所开发的壳程序（shell）及脚本语言技术，采用的是命令行界面。这项全新的技术提供了丰富的控制与自动化的系统管理能力。

PowerShell 使用 C# 编写，采用MIT许可协议，可安装在 Windows, OS X 和 Linux 操作系统上。

[PowerShell文档](https://github.com/PowerShell/PowerShell-Docs)

### Mono
Mono 是原始的跨平台和 开放源 .NET 实现，于 2004 年首次发布。 可以把它看作是 .NET Framework 的社区克隆。 Mono 项目团队依赖于 Microsoft 发布的开放 .NET Standard（尤其是 ECMA 335），以便实现兼容性。 

.NET Core 和 Mono 的主要差异在于：
* 应用模型 -- Mono 通过 Xamarin 产品支持 .NET Framework 应用模型（例如，Windows Forms）和其他应用模型（例如，Xamarin.iOS）的子集。 而 .NET Core 不支持这些内容。
* API -- Mono 使用相同程序集名称和组成要素支持 .NET Framework API 的 大型子集。
* 平台 -- Mono 支持很多平台和 CPU。
* 开放源码 -- Mono 和 .NET Core 两者都使用 MIT 许可证，且都属于 .NET Foundation 项目。
* 焦点 --最近几年，Mono 的主要焦点是移动平台，而 .NET Core 的焦点是云工作负荷。

### 组成
[.NET 标准库](https://docs.microsoft.com/zh-cn/dotnet/articles/standard/library)是一组由 .NET 运行时实现的 API，正式项目：CoreFX。

[ECMA 335](https://github.com/dotnet/coreclr/blob/master/Documentation/project-docs/dotnet-standards.md) 持续为 .NET 运行时行为建立统一性，但适用于 .NET 库实现的 .NET 基类库 (BCL) 没有类似的规范。

Microsoft 积极开发和维护的主要 .NET 运行时有 3 个：.NET Core、.NET Framework 和 Mono for Xamarin。

CLR(Common Language Runtime)的主要功能如下：
* 基类库支持 Base Class Library Support
* 内存管理 Memory Management
* 线程管理 Thread Management
* 垃圾回收 Garbage Collection
* 安全性 Security
* 类型检查 Type Checker
* 异常管理 Exception Manager
* 除错管理 Debug Engine
* 中间码(MSIL)到机器码(Native)编译
* 类装载 Class Loader

### 核心项目
* [.NET Core Libraries (CoreFX)](https://github.com/dotnet/corefx) 主要由C#编写
* [.NET Core Runtime (CoreCLR)](https://github.com/dotnet/coreclr) 主要由C++编写
* [.NET Compiler Platform (Roslyn)](https://github.com/dotnet/roslyn) 主要由C#编写
* [LLILC](https://github.com/dotnet/llilc) is an LLVM based MSIL Compiler 主要由C++编写
* [.NET Command Line Interface(CLI tools)](https://github.com/dotnet/cli) 主要由C#编写

### 核心语言
.NET平台的核心：C# 和 F#

C#是微软推出的一种基于.NET框架的、面向对象的高级编程语言。C#由C语言和C++派生而来，继承了其强大的性能，同时又以.NET 框架类库作为基础，拥有类似Visual Basic的快速开发能力。

F#(F sharp)是由微软发展的为.NET语言提供运行环境的程序设计语言，是一门函数式编程语言（FP，Functional programming），函数式编程语言最重要的基础是Lambda Calculus。

F#和OCaml 是ML函数式编程语言的两种主要方言，有时F#和OCaml的程序是可以交互编译的。

F# 采用 MIT 许可协议。

### Q#
Q#是微软推出的量子编程语言，它依赖于C#和F#。

从[如何评价微软刚刚发布的量子编程语言 Q# ？](https://www.zhihu.com/question/263946287/answer/287593143)先多了解一些Q#语言的背景。

### 案例
* [On how Jet chose F#](https://tech.jet.com/blog/2015/03-22-on-how-jet-chose/), [Jet @ GitHub](https://github.com/jet)
* [瑞信](https://www.credit-suisse.com/cn/sc.html) [Quantitative Finance in F#](http://fsharp.org/testimonials/#credit-suisse-abstract) Why FP matters to Credit Suisse
* 沪牌拍牌系统后台是.NET写的，并发至少几千每秒，这个大家懂的；Stackoverflow核心是.NET写的，网站并发 3000每秒，数据库并发 8000每秒；摩根斯坦利交易客户端以及协议是.NET写的；NASDAQ的交易系统是.NET写的，后台跑的SQL Server；腾讯有大量后台系统用.NET写，腾讯甚至已经使用跨平台.NET（Mono）很多年，部署于它的TLinux系统集群中；携程有大量系统用.NET写成，日均动态PV是3千万。 来源：[NET技术在中国为什么老被人嫌弃](https://www.cnblogs.com/neuzilla/p/dotnet_china_market_share.html)

### 文档
* [Why FP matters to Credit Suisse](http://docs.huihoo.com/cufp/2004-2008/2006/slides/HowardMansell.pdf)
* [F# for fun and profit](http://book.huihoo.com/dotnet/fsharp-for-fun-and-profit.pdf)

### 图集
![.NET](https://wiki.huihoo.com/images/thumb/8/8a/Dotnet-components.png/1280px-Dotnet-components.png).NET体系结构组件

![ASP.NET](https://wiki.huihoo.com/images/8/86/ASPNET-IIS-Execute.png)ASP.NET运行架构

![ASP.NET Core](https://wiki.huihoo.com/images/9/94/ASP.NET-Core-Component.jpg)ASP.NET Core组件

![CLR](https://wiki.huihoo.com/images/thumb/e/e8/Common-Language-Runtime.png/1280px-Common-Language-Runtime.png)Common Language Runtime(CLR)

![.NET性能](https://wiki.huihoo.com/images/5/54/Dotnet-performance.png)在这里只想说.NET平台性能真还不错 :)

![F# finance](https://wiki.huihoo.com/images/f/f8/Fsharp-finance-data.png)F#金融数据

![F# data](https://wiki.huihoo.com/images/thumb/e/e1/Fsharp-data-science-with-fsLab-and-ionide.png/1280px-Fsharp-data-science-with-fsLab-and-ionide.png)F#数据科学

### 链接
* [.NET Foundation](https://github.com/dotnet)
* [.NET官网](https://dotnet.microsoft.com/)
* [ASP.NET官网](https://www.asp.net/)
* [C#指南](https://docs.microsoft.com/zh-cn/dotnet/csharp/)
* [F#官网](http://fsharp.org/)
* [PowerShell官网](https://microsoft.com/powershell%20)

## 许可方式 License

课程和课件采用CC

[![CC](http://wiki.huihoo.com/images/4/4e/CC-BY-SA_3.0-88x31.png)](http://wiki.huihoo.com/wiki/CC-BY-SA_3.0)

代码采用MIT

## 赞助与支持
本服务教程为免费教程，若需要得到更多技术支持，可通过赞助我们的方式获得。

![灰狐会员](http://wiki.huihoo.com/images/2/25/Zsxq.jpg)

[灰狐会员](https://wiki.huihoo.com/wiki/%E7%81%B0%E7%8B%90%E4%BC%9A%E5%91%98)





