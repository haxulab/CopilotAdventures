## 斯通维尔的传奇决斗

<a href="#">
    <img src="../../Images/stonevale.jpg" style="width: 830px" />
</a>

### 背景

在神秘的斯通维尔王国，两位战士Rok和Papyra被选中进行一场决斗，这场决斗决定他们部落在接下来一个世纪的命运。竞技场称为Scissoria，在那里每一个动作都有其意义和后果。

### 目标

你的任务是模拟Rok和Papyra之间的决斗。每位战士进行一系列动作，每个动作都有特定的结果。赢得决斗的战士必须在一系列回合中积累最高分。

### 规格

1. **动作和分数：**
    - 每位战士可以做出三个动作之一：石头，剪刀或布。
        - 石头赢 = 1分
        - 布赢 = 2分
        - 剪刀赢 = 3分

1. **决斗动态：**
    - 当两位战士选择相同的动作时，结果为平局，不得分。
    - 石头砸碎剪刀，布包住石头，剪刀剪开布。
    - 根据胜利的动作授予分数。

1. **游戏玩法：**
    - 决斗由5回合组成。
    - 目标是在这些回合中积累最高分以赢得决斗。

1. **玩家动作：**

    **Rok（玩家1）的动作**

    | 第1回合 | 第2回合 | 第3回合 | 第4回合 | 第5回合 |
    |---------|---------|---------|---------|---------|
    | 剪刀    | 布      | 剪刀    | 石头    | 石头    |

    **Papyra（玩家2）的动作**

    | 第1回合 | 第2回合 | 第3回合 | 第4回合 | 第5回合 |
    |---------|---------|---------|---------|---------|
    | 石头    | 石头    | 布      | 剪刀    | 布      |

1. **高级功能（如果有时间）：**
    - 实现一个建议系统，向玩家建议一个动作。
    - 玩家可以在每一回合选择他们的动作，而不是自动化的。

### 约束

- 使用GitHub Copilot和任何你选择的语言编写模拟。尝试学习一种新语言，如果你准备好了挑战！
- 确保高效的算法处理决斗动态。询问GitHub Copilot/Chat，“如何使这段代码更易读和可维护？”。
- 提供图形用户界面进行模拟是可选的。

### 执行高层任务的摘要

1. 使用控制台应用程序渲染输出。
1. 初始化两位战士的分数。
1. 每个战士为每回合选择一个动作。
1. 确定每回合的获胜者并授予分数。
1. 在五回合后累计分数。
1. 宣布决斗的总体胜利者。

### 如何开始的小贴士

1. 如果你正在使用GitHub Codespace，你已经准备好了！
1. 如果在本地运行，请确保你已安装你的目标语言/框架。
    - [Node.js](https://nodejs.org)
    - [Python](https://www.python.org/downloads/)
    - [.NET](https://dot.net)
1. 创建一个代码文件夹。
    - JavaScript：创建一个名为`stonevale`的文件夹，并添加一个名为`app.js`的文件。
    - Python：创建一个名为`stonevale`的文件夹，并添加一个名为`app.py`的文件。
    - C#：创建一个名为`stonevale`的文件夹，并运行`dotnet new console`。

### GitHub Copilot 提示

<a href="#">
    <img src="../../Images/copilot-tips.jpg"  style="width: 830px" />
</a>

#### 使用Copilot提高效率

查看是否可以使用Copilot找到代码的复杂度（BigO表示法）。

1. 在侧边栏打开[GitHub Copilot Chat视图](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat#asking-your-first-question)，如果它还没有打开的话。确保解决方案文件也仍然打开。

1. 询问Copilot Chat代码的复杂度。

1. 询问Copilot Chat怎样使代码更加高效。

1. 再次询问复杂度——是否有所改进？

#### 使用Copilot生成代码注释

1. 使用<kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>A</kbd>高亮所有代码。

1. 按<kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>I</kbd>打开内联聊天。

1. 输入"/doc"

1. 询问Copilot Chat为函数编写文档。

#### 使用Copilot简化代码

1. 打开侧边栏的GitHub Copilot Chat。

1. 输入"/simplify"并按<kbd>Enter</kbd>。你也可以在"/simplify"后添加任意文本，给Copilot更多指示。

1. Copilot Chat建议你做什么来简化代码？

#### 出错了？

Copilot Chat也可以帮助解决这个问题！只需复制错误信息并粘贴到聊天中。通常这已经足够让Copilot解决问题。