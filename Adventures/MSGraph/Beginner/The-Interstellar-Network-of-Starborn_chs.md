## 星际网络

![星生](../../../Images/starborn.jpg)

### 背景

在一个遥远的宇宙中，各个文明已经发展到跨星际旅行并定居在遥远星球上变得司空见惯的地步。每个星球都居住着“星生”，即根据他们的新家园星球调整和进化的人类。

星生文明通过一个庞大的数字网络——“星际网络”连接在一起。这个网络的主要目的是维护每个星生及其在星际社区中角色的记录。

就像行星和恒星有各自的轨道和层级，星生也有自己的层级。每个星生都有一个直接上司，他们向其汇报工作，这一链条最终汇报给星生文明的领袖——宇宙大统领。

### 目标

你是一名新任命的星球Azurea的系统管理员。你的第一个任务是访问星际网络租户并执行以下任务：

1. 通过[访问他们的网站](https://developer.microsoft.com/microsoft-365/dev-program)并加入该计划，创建一个星际网络租户（如果你还没有的话）。
1. 研究[文档](https://learn.microsoft.com/training/paths/m365-msgraph-fundamentals/)，学习如何访问星际网络。
1. 尽管星际网络极其先进，他们仍然使用HTML和JavaScript。要与他们的网络互动，请创建一个简单的HTML页面，并使用JavaScript实现以下功能：
    - 使用星生凭证登录星际网络。
    - 显示你的个人信息。
    - 确定并展示你在星际层级中直接汇报的上司。

### 规范

1. **登录**：
    - 访问星际网络并使用你的星生凭证登录。
    - 检索并显示你的资料，确保你访问的是正确的账户。

1. **层级查询**：
    - 登录后，使用网络确定你直接汇报给谁。
    - 显示你直接汇报的上司的资料。

1. **API端点**：
    - 使用`/me`端点检索你的星际网络资料。
    - 使用`/me/manager`端点检索你直接上司的资料。

### 约束

- 编写一个控制台应用程序。
- 使用Microsoft Graph API与星际网络互动。
- 确保安全且高效地访问网络。
- 优雅地处理任何潜在的错误或访问问题。

### 高级任务摘要

1. 使用`/me`端点进行API调用以登录并检索你的资料。
2. 显示你的个人信息。
3. 使用`/me/manager`端点进行另一次API调用以确定你的直接上司。
4. 显示你直接上司的资料。

### 示例数据

登录星际网络后，你的个人资料将遵循以下格式：

```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "businessPhones": [
        "+1 412 555 0109"
    ],
    "displayName": "Megan Bowen",
    "givenName": "Megan",
    "jobTitle": "Auditor",
    "mail": "MeganB@M365x214355.onmicrosoft.com",
    "mobilePhone": null,
    "officeLocation": "12/1110",
    "preferredLanguage": "en-US",
    "surname": "Bowen",
    "userPrincipalName": "MeganB@M365x214355.onmicrosoft.com",
    "id": "48d31887-5fad-4d73-a9f5-3c356e68a038"
}
```