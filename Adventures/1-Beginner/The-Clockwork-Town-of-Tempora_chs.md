## 天机镇

<a href="#">
    <img src="../../Images/tempora-clocks.jpg"  style="width: 830px" />
</a>

### 背景

在机械小镇天机镇里，一切都依靠钟表和精确的时机来运转。小镇的中心是大钟塔，它负责为小镇的所有活动提供时间。然而，随着时间推移，小镇中的一些小钟表开始偏离准确时间。

### 目标

你的任务是创建一个系统来检查小镇中的所有钟表，并将它们与大钟塔同步。你将获得一份来自小镇各处钟表的时间列表，你必须确定每个钟表比大钟塔的时间快了或慢了多少分钟。

### 规格

1. **钟表数据：**
    - 钟表时间以24小时制提供。
    - 大钟塔的时间是15:00。
    - 小镇中各钟表时间：
        - 钟表 1: 14:45
        - 钟表 2: 15:05
        - 钟表 3: 15:00
        - 钟表 4: 14:40

2. **时间分析与输出：**
    - 你需要确定每个钟表比大钟塔快了或慢了多少分钟。
    - 结果应为一个整数数组，表示时间差（单位为分钟）。正值表示钟表快，负值表示钟表慢。

### 约束条件

- 使用GitHub Copilot并使用你喜欢的任何语言编写模拟程序。
- 重点在于代码的清晰和简洁。可以询问GitHub Copilot/Chat，“如何使这段代码更可读和更易维护？”。
- 创建钟表的可视化表示是可选的，但如果有时间鼓励你去尝试。

### 高级任务概览

1. 使用控制台应用程序渲染输出。
1. 解析各个钟表和大钟塔的时间数据。
1. 计算每个钟表与大钟塔之间的时间差（分钟）。
1. 输出时间差列表。

### 入门提示

1. 如果你在使用GitHub代码空间，你已经准备好了！
1. 如果在本地运行，确保你已经安装了目标语言/框架。
    - [Node.js](https://nodejs.org)
    - [Python](https://www.python.org/downloads/)
    - [.NET](https://dot.net)
1. 创建一个代码文件夹。
    - JavaScript: 创建一个名为`tempora`的文件夹，并添加一个名为`app.js`的文件。
    - Python: 创建一个名为`tempora`的文件夹，并添加一个名为`app.py`的文件。
    - C#: 创建一个名为`tempora`的文件夹，并运行`dotnet new console`。

### GitHub Copilot 提示

<a href="#">
    <img src="../../Images/copilot-tips.jpg"  style="width: 830px" />
</a>

#### 使用Copilot提高效率

看看你能否使用Copilot来确定代码的复杂度（大O标记）。

1. 在侧边栏中打开[GitHub Copilot Chat视图](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat#asking-your-first-question)（如果还没有打开）。确保你的解决方案文件也是打开的。

1. 向Copilot Chat询问代码的复杂度。

1. 向Copilot Chat询问如何使代码更高效。

1. 再次询问复杂度 - 是否变得更好了？

#### 使用Copilot生成代码注释

1. 使用<kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>A</kbd>选择所有代码。

1. 按<kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>I</kbd>打开内联聊天。

1. 输入“/doc”

1. 向Copilot Chat请求函数的文档。

#### 使用Copilot简化代码

1. 在侧边栏中打开GitHub Copilot Chat。

1. 输入“/simplify”并按<kbd>Enter</kbd>。你也可以在“/simplify”之后添加任何文本，以给Copilot更多的指示。

1. Copilot Chat建议你怎么做以使代码更简洁？

#### 遇到错误？

Copilot Chat也可以帮助你解决问题！只需复制错误信息并粘贴到Chat中。通常，这就是Copilot解决问题所需的全部信息。