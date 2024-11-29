## Eldoria的卷轴

<a href="#">
    <img src="../../Images/eldoria.jpg" style="width: 830px" />
</a>

### 背景

在魔法之地Eldoria，古老的卷轴蕴含着宇宙的秘密。然而，这些卷轴很久以前被长老们用强大的咒语散布并保护起来。这些咒语掩盖了卷轴中的秘密，增加了误导性的信息以阻止窥探者。随着时间的推移，这些卷轴被数字化并存储在伟大的Eldoria图书馆中，只能通过Eldoria知识网络访问。

### 任务目标

你，作为一名年轻的魔法学徒，被赋予了取回并破解其中一个卷轴的任务。这个卷轴作为一个文件存储在Eldoria知识网络上。你需要进行一个HTTP调用来获取卷轴的内容。然而，必须使用古老的正则表达式方法过滤掉长老们的误导性信息，以揭示其中的真正秘密。

### 规格

1. **数据检索：**
    - 使用魔法HTTP调用来获取卷轴的内容。你将在伟大的Eldoria图书馆的 `https://raw.githubusercontent.com/microsoft/CopilotAdventures/main/Data/scrolls.txt` 位置找到卷轴。
    - 内容将以文本格式提供。

2. **破解卷轴：**
    - 卷轴包含长老们的秘密和误导性信息。
    - 真正的秘密有一个特定的模式：总是被符号 `{*` 和 `*}` 围绕。
    - 提取卷轴中所有的真正秘密。

3. **输出：**
    - 以结构化的方式显示提取的秘密。
    - 确保不会显示误导性信息。

### 约束条件

- 使用GitHub Copilot和任何你选择的语言编写模拟程序。如果你愿意接受挑战，可以尝试学一门新语言！
- 确保使用高效的算法来处理文本的检索和提取。问GitHub Copilot/Chat：“如何使这段代码更具可读性和可维护性？”

### 要执行的高层次任务摘要

1. 使用控制台应用程序来呈现输出。
1. 进行HTTP调用以检索卷轴内容。
1. 使用正则表达式过滤掉误导性信息并提取真正的秘密。
1. 显示提取的秘密。

### 入门提示

1. 如果你使用的是GitHub Codespace，你已经准备好了！
1. 如果在本地运行，确保你安装了目标语言/框架。
    - [Node.js](https://nodejs.org)
    - [Python](https://www.python.org/downloads/)
    - [.NET](https://dot.net)
1. 创建一个文件夹用于代码。
    - JavaScript：创建一个名为 `eldoria` 的文件夹并添加一个名为 `app.js` 的文件。
    - Python：创建一个名为 `eldoria` 的文件夹并添加一个名为 `app.py` 的文件。
    - C#: 创建一个名为 `eldoria` 的文件夹并运行 `dotnet new console`。

### GitHub Copilot 提示

<a href="#">
    <img src="../../Images/copilot-tips.jpg"  style="width: 830px" />
</a>

#### 使用Copilot提高效率

看看你能否使用Copilot找出代码的复杂度（BigO notation）。

1. 打开侧边栏中的 [GitHub Copilot Chat视图](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat#asking-your-first-question)，如果尚未打开的话。确保你的解决方案文件仍然是打开的。

1. 问Copilot Chat代码的复杂度是多少。

1. 问Copilot Chat如何使代码更高效。

1. 再次询问复杂度——是否有所改善？

#### 使用Copilot生成代码注释

1. 使用 <kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>A</kbd> 高亮所有代码。

1. 按 <kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>I</kbd> 打开内嵌聊天。

1. 输入 "/doc"

1. 让Copilot Chat为函数编写文档。

#### 使用Copilot简化代码

1. 在侧边栏中打开GitHub Copilot Chat。

1. 输入 "/simplify" 并按 <kbd>Enter</kbd>。你也可以在"/simplify"之后添加任何文本以提供更多指示给Copilot。

1. Copilot Chat建议你如何简化代码？

#### 遇到错误？

Copilot Chat也能帮忙！只需复制错误信息并粘贴到聊天中。通常这已经足够让Copilot解决你的问题。