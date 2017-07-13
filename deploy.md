#服务发布

## 动机

部署一个单体应用意味着对一个一般比较庞大的应用运行多个相同的拷贝，通常需要提供N台服务器（物理机或者虚拟机），并在每一台机器上运行M个应用实例。部署一个单体应用一般并不是特别直接，但是相比部署微服务架构的应用来讲，它已经简单很多了。

一个微服务应用包含数十个甚至上百个服务，服务是由多种不同的编程语言和框架写成，每一个服务都是一个有自己独特的部署、资源、扩展性以及监控需求的mini应用。比如，你需要根据服务的需求对该服务运行一定数量的实例，而且，每一个服务实例必须提供适当的CPU、内存以及I/O资源，更加具有挑战性的是，尽管这很复杂，部署一个服务同时还要求 快速、可靠、高效。

## 基于容器的发布部署


### 打包发布

- 服务端代码
通过持续集成将验证后的正式版程序推送存储到线上的代码仓库系统

- 前端代码
通过持续集成后将编译后的代码发布到线上cdn系统

- 配置及密钥
配置及密钥存储于线上密钥仓库sercet，只能指定人员编辑


### 部署生效
