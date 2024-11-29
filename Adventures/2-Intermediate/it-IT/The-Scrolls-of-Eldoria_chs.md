## 伊尔多利亚的卷轴

<a href="#">
    <img src="../../../Images/eldoria.jpg" style="width: 830px" />
</a>

### 背景

在被魔法笼罩的伊尔多利亚大陆，古老的卷轴中包含着宇宙的秘密。然而，这些卷轴被长老们使用强大的法术分散并保护起来。这些法术隐匿了卷轴中的秘密，加入了误导信息，以阻止不慎之人窥探。随着时间的推移，这些卷轴已经被数字化并保存在伊尔多利亚的大图书馆中，只能通过伊尔多利亚知识网络访问。

### 目标

你，作为一名年轻的巫师学徒，接到了任务去回收并解读其中的一卷。卷轴作为一个文件保存在伊尔多利亚知识网络中。你需要进行一次HTTP请求来获取卷轴的内容。然而，必须使用古老的正则表达式方法来过滤长老们的误导信息，以揭示卷轴中真正的秘密。

### 规范

1. **数据获取:**
    - 使用魔法的HTTP请求来获取卷轴的内容。你可以在伊尔多利亚大图书馆的这个位置找到卷轴 `https://raw.githubusercontent.com/microsoft/CopilotAdventures/main/Data/scrolls.txt`。
    - 内容将是文本格式。

2. **解读卷轴:**
    - 卷轴包含长老们的秘密以及误导信息。
    - 真正的秘密有一个特定的模式：始终被 `{*` 和 `*}` 符号包围。
    - 从卷轴中提取所有真正的秘密。

3. **输出:**
    - 以结构化的方式显示提取的秘密。
    - 确保没有展示误导信息。

### 约束

- 使用GitHub Copilot以及你选择的任何语言来编写模拟。若你准备好迎接挑战，请尝试学习一种新语言！
- 确保使用高效的算法来处理文本获取及提取。可以咨询GitHub Copilot/Chat，“如何使这个代码更具可读性和可维护性？”。

### 高级任务的总结

1. 使用控制台应用程序来显示输出。
1. 进行一次HTTP请求来获取卷轴的内容。
1. 使用正则表达式过滤误导信息并提取真正的秘密。
1. 显示提取的秘密。

### 开始提示

1. 如果你在使用GitHub Codespace，你已经准备好了！
1. 如果你在本地运行，请确保已安装目标语言/框架。
    - [Node.js](https://nodejs.org)
    - [Python](https://www.python.org/downloads/)
    - [.NET](https://dot.net)
1. 创建一个文件夹来保存你的代码。
    - JavaScript: 创建一个名为 `eldoria` 的文件夹，并添加一个名为 `app.js` 的文件。
    - Python: 创建一个名为 `eldoria` 的文件夹，并添加一个名为 `app.py` 的文件。
    - C#: 创建一个名为 `eldoria` 的文件夹，并运行 `dotnet new console`。

### 使用GitHub Copilot的提示

<a href="#">
    <img src="../../../Images/copilot-tips.jpg"  style="width: 830px" />
</a>

#### 使用Copilot提升效率

看看能否使用Copilot来发现代码的复杂度（大O记号）。

1. 如果尚未打开，请在侧边栏中打开[GitHub Copilot聊天视图](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat#asking-your-first-question)。确保解决方案文件仍然打开。
2. 向Copilot Chat询问代码的复杂度。
3. 向Copilot Chat询问如何使代码更加高效。
4. 再次询问复杂度——是否有所改善？

#### 使用Copilot生成代码注释

1. 用 <kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>A</kbd> 高亮所有代码。
2. 按 <kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>I</kbd> 打开内联聊天。
3. 输入 "/doc"
4. 让Copilot Chat为函数生成文档。

#### 使用Copilot简化代码

1. 在侧边栏打开GitHub Copilot聊天。
2. 输入 "/simplify" 并按 <kbd>Enter</kbd>。你也可以在 "/simplify" 后添加任何你希望的文本，以给予Copilot更多指示。
3. Copilot Chat为你简化代码做了什么建议？

#### 遇到错误了？

Copilot Chat也可以帮助你！只需复制错误提示并粘贴到聊天中。这通常是Copilot解决你问题所需的全部信息。