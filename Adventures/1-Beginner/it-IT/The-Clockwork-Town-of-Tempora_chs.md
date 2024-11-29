## 机械城 Tempora

<a href="#">
    <img src="../../../Images/tempora-clocks.jpg" style="width: 830px" />
</a>

### 背景

在机械城Tempora，一切都按照时钟精确运行。在城镇中心坐落着大钟塔，负责管理整个城市的时间。然而，多年来，城市中的一些小钟表开始偏离标准时间。

### 目标

你的任务是创建一个系统，用来检查城镇中的所有钟表并将它们与大钟塔同步。你将获得一些来自城市各处钟表的时间列表，需要确定每个钟表相对于大钟塔的时间快了或慢了多少分钟。

### 规格

1. **钟表数据:**
    - 钟表时间以24小时制格式提供。
    - 大钟塔的时间是15:00。
    - 城市中的各个钟表时间：
        - 钟表1：14:45
        - 钟表2：15:05
        - 钟表3：15:00
        - 钟表4：14:40

2. **时间分析和输出:**
    - 你需要确定每个钟表相对于大钟塔时间快了或慢了多少分钟。
    - 结果应该是一个整数数组，表示时间差异，正值表示钟表快，负值表示钟表慢。

### 约束

- 使用GitHub Copilot并用你喜欢的任何编程语言编写该模拟。
- 关注简洁明了的代码。请使用GitHub Copilot/Chat询问，“怎样使这段代码更可读和可维护？”。
- 如果有时间，创建一个钟表的可视化表示是可选但鼓励的。

### 高级任务总结
1. 使用控制台应用程序显示输出。
2. 分析每个钟表和大钟塔的时间数据。
3. 计算每个钟表和大钟塔之间的分钟差异。
4. 显示时间差异列表。

### 入门提示

1. 如果你在使用GitHub Codespace，那你已经准备好了开始！
1. 如果你在本地工作，确保安装了目标语言/框架。
    - [Node.js](https://nodejs.org)
    - [Python](https://www.python.org/downloads/)
    - [.NET](https://dot.net)
1. 创建一个代码文件夹。
    - JavaScript：创建一个名为`tempora`的文件夹，并添加一个名为`app.js`的文件。
    - Python：创建一个名为`tempora`的文件夹，并添加一个名为`app.py`的文件。
    - C#：创建一个名为`tempora`的文件夹，并运行`dotnet new console`。

### GitHub Copilot 建议

<a href="#">
    <img src="../../../Images/copilot-tips.jpg" style="width: 830px" />
</a>

#### 使用Copilot 提高效率

看看你是否可以使用Copilot发现代码的复杂度（BigO表示法）。

1. 打开侧栏中的[GitHub Copilot聊天视图](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat#asking-your-first-question)，如果还没打开。确保你的解决方案文件仍然打开着。

1. 向Copilot Chat询问代码的复杂度。

1. 向Copilot Chat询问如何使代码更高效。

1. 再次询问复杂度——是否有所改善？

#### 使用Copilot生成代码注释

1. 使用<kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>A</kbd>选择所有代码。

1. 按<kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>I</kbd>以打开内联聊天。

1. 输入"/doc"
1. 向Copilot Chat询问如何为函数添加注释。

#### 使用Copilot 简化你的代码

1. 打开侧栏中的GitHub Copilot聊天视图。

1. 输入"/simplify"并按<kbd>Enter</kbd>。你也可以在"/simplify"后添加任何你想要的文本以给Copilot更多指令。

1. Copilot Chat建议了什么来简化代码？

#### 是否有错误？

Copilot聊天也能帮助你！只需复制错误信息并将其粘贴到聊天中。通常这就是Copilot解决问题所需要的全部信息。