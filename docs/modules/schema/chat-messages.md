---
hide_table_of_contents: true
sidebar_position: 3
---

# 聊天消息

终端用户与LLMs互动的主要界面是聊天界面。因此，一些模型提供商已经开始以期望聊天消息的方式提供对底层API的访问。这些消息具有内容字段（通常是文本)，并与用户（或角色)相关联。当前支持的用户有System， Human，和AI。

## SystemMessage

表示应为AI系统提供说明的聊天消息。

```类型脚本
import { SystemMessage } from "langchain/schema";



new SystemMessage("You are a nice assistant");

```


## HumanMessage

表示来自与AI系统交互的人的信息的聊天消息。

```类型脚本
import { HumanMessage } from "langchain/schema";



new HumanMessage("Hello, how are you?");

```


## AIMessage

表示来自AI系统的消息的聊天消息。

```typescript

import { AIMessage } from "langchain/schema";



new AIMessage("I am doing well, thank you!");

```

