## 石谷的传奇决斗

<a href="#">
    <img src="../../../Images/stonevale.jpg" style="width: 830px" />
</a>

### 背景

在神秘的石谷王国，两位战士Rok和Papyra被选中进行一场决斗，这场决斗将决定他们部落在接下来一个世纪的命运。竞技场，名为Scissoria，是每一步都有重量和后果的地方。

### 目标

你的任务是模拟Rok和Papyra之间的决斗。每个战士进行一系列的动作，每个动作都有特定的结果。要赢得决斗，一个战士必须在一系列回合中积累最高的分数。

### 规格

1. **动作和得分:**
    - 每个战士可以进行三种动作之一：石头，纸或剪刀。
        - 用石头获胜 = 1 分
        - 用纸获胜 = 2 分
        - 用剪刀获胜 = 3 分

1. **决斗动态:**
    - 当两个战士选择相同的动作时，是平局，不会被分配分数。
    - 石头砸剪刀，纸包石头，剪刀剪纸。
    - 根据获胜的动作分配分数。

1. **游戏模式:**
    - 决斗由5个回合组成。
    - 目标是在这些回合中积累最高的分数以赢得决斗。

1. **玩家的动作：**

    **Rok的动作 (玩家1)**

    | 第一回合 | 第二回合 | 第三回合 | 第四回合 | 第五回合 |
    |---------|---------|---------|---------|---------|
    | 剪刀    | 纸   | 剪刀| 石头    | 石头   |

    **Papyra的动作 (玩家2)**

    | 第一回合 | 第二回合 | 第三回合 | 第四回合 | 第五回合 |
    |---------|---------|---------|---------|---------|
    | 石头 | 石头    | 纸   | 剪刀| 纸    |


1. **高级功能 (如有时间):**
    - 实现一个提示系统，给玩家建议一个动作。
    - 玩家可以为每个回合选择自己的动作，而不是自动化的。

### 约束

- 使用GitHub Copilot并选择任何语言编写模拟程序。如果你准备好了挑战，尝试学习一种新的语言！
- 确保使用高效的算法来处理决斗的动态。问问GitHub Copilot/Chat，“如何使这个代码更易读和更可维护？”
- 提供图形界面来进行模拟是可选的。

### 需要执行的高级别任务摘要

1. 使用控制台应用程序显示输出。
1. 初始化两个战士的分数。
1. 每个战士为每个回合选择一个动作。
1. 确定每个回合的胜者并分配分数。
1. 五个回合后统计分数。
1. 宣布决斗的总胜者。

### 入门提示

1. 如果你正在使用GitHub Codespace，你已经准备好了！
1. 如果你在本地运行，请确保安装了你的目标语言/框架。 
    - [Node.js](https://nodejs.org)
    - [Python](https://www.python.org/downloads/)
    - [.NET](https://dot.net)
1. 创建一个用于存放代码的文件夹。 
    - JavaScript: 创建一个名为`stonevale`的文件夹并添加一个名为`app.js`的文件。
    - Python: 创建一个名为`stonevale`的文件夹并添加一个名为`app.py`的文件。
    - C#: 创建一个名为`stonevale`的文件夹并运行`dotnet new console`。

### GitHub Copilot 提示

<a href="#">
    <img src="../../../Images/copilot-tips.jpg"  style="width: 830px" />
</a>

#### 使用 Copilot 提高效率

看看你能不能用 Copilot 来发现代码的复杂度（BigO表示法）。

1. 打开侧边栏中的 [GitHub Copilot Chat 视图](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat#asking-your-first-question)。确保你的解决方案文件仍然打开。
2. 向 Copilot Chat 询问代码的复杂度。
3. 让 Copilot Chat 使代码更高效。
4. 再次询问代码复杂度——有没有改善？

#### 使用 Copilot 生成代码注释

1. 按 <kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>A</kbd> 全选所有代码。
2. 按 <kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>I</kbd> 打开inline聊天窗口。
3. 输入 "/doc"
4. 让 Copilot Chat 为函数生成文档。

#### 使用 Copilot 简化你的代码

1. 打开侧边栏中的 Copilot Chat。
2. 输入 "/simplify" 并按 <kbd>Enter</kbd>。您还可以在 "/simplify" 后面添加任何你想要的说明以给 Copilot 更多指导。
3. Copilot Chat 建议你用什么来简化代码？

#### 有错误？

Copilot Chat 也可以帮你解决！只是将错误消息复制粘贴到Chat中。通常这就是Copilot需要解决你的问题的一切。