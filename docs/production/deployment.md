## 部署

您已经构建好了 LangChain 应用程序，并且现在想将其部署到生产环境？您来对地方了。本指南将为您介绍部署应用程序的选项以及进行部署时应考虑的问题。

## 概述

LangChain 是用于构建使用语言模型的应用程序的库。它不是 Web 框架，并且不提供任何用于通过 Web 提供服务的内置功能。相反，它提供了一组工具，您可以将其集成在 API 或后端服务器中。

部署应用程序有几个高级选项:

- 部署到虚拟机或容器中
  - Persistent filesystem means you can save and load files from disk

  - Always-running process means you can cache some things in memory

  - You can support long-running requests, such as WebSockets

- 部署到无服务器环境
  - No persistent filesystem means you can load files from disk, but not save them for later

  - Cold start means you can't cache things in memory and expect them to be cached between requests

  - Function timeouts mean you can't support long-running requests, such as WebSockets


其他一些考虑事项包括:

- 您将后端和前端一起部署还是分别部署？
- 您将后端与数据库协同部署还是分别部署？

随着您将 LangChain 应用程序部署到生产环境，我们将非常乐意提供更全面的支持。请填写 [此表格](https://forms.gle/57d8AmXBYp8PP8tZA)，我们将设置一个专门的支持 Slack 频道。

## 部署选项

请参阅以下有关 LangChain 应用程序部署选项的列表。如果您没有看到您首选的选项，请联系我们，我们可以将其添加到此列表中。

### 部署到 Fly.io

[Fly.io](https://fly.io) 是将应用程序部署到云端的平台。这是将您的应用程序部署到容器环境的不错选择。

请参阅 [我们的 Fly.io 模板](https://github.com/hwchase17/langchain-template-node-fly) ，其中包含了将应用程序部署到 Fly.io 的示例。

### 部署到 Kinsta


[Kinsta](https://kinsta.com)是一个以开发人员为中心的云主机平台。


Use [our hello-world template](https://github.com/kinsta/hello-world-langchainjs) for an example of how to deploy your next LangChain app at Kinsta in minutes.

