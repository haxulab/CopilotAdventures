## 魔法森林Algora

<a href="#">
    <img src="../../../Images/algora-forest.jpg" style="width: 830px" />
</a>

### 背景

在神秘的Algora森林深处，每千年两只神奇的生物Lox和Faelis都会进行一场神圣的舞蹈。这舞蹈不仅是一种庆祝，更是恢复森林平衡的仪式。

### 目标

你的任务是模拟Lox和Faelis的舞蹈。每个生物都有自己的一套舞步组合，而这些组合在森林中创造出各种魔法效果。你的目标是确定舞蹈完成后森林的状态。

### 规范

1. **舞步及效果：**
    - 每个生物可以执行三种舞步之一：`旋转`、`跳跃`或`滚动`。
    - 两个生物的舞步组合会产生魔法效果：
        - 旋转 + 旋转 = 萤火虫点亮森林。
        - 跳跃 + 滚动 = 开始下起小雨。
        - 滚动 + 跳跃 = 天上出现彩虹。
        - 其他组合会产生不同效果，具体效果由你想象。

2. **舞蹈动态：**
    - 每个效果都会改变森林的状态。
    - 有些效果可能是有益的，而另一些可能是有害的。

3. **舞蹈序列：**
    - 舞蹈由5个序列组成。
    - 你需要展示每个序列后的森林状态。

4. **生物的舞步：**

    **Lox (生物1)的舞步**

    | 序列1   | 序列2   | 序列3   | 序列4   | 序列5   |
    |---------|---------|---------|---------|---------|
    | 旋转    | 跳跃    | 滚动    | 旋转    | 跳跃    |

    **Faelis (生物2)的舞步**
    | 序列1   | 序列2   | 序列3   | 序列4   | 序列5   |
    |---------|---------|---------|---------|---------|
    | 滚动    | 旋转    | 跳跃    | 跳跃    | 滚动    |

5. **高级功能（如果时间允许）：**
    - 实现一个系统，允许用户添加新的舞步和效果。
    - 用户可以为每个序列选择舞步。

### 约束

- 使用GitHub Copilot编写模拟代码，语言不限。
- 注重代码的清晰简洁，确保舞蹈动态处理高效。可以向GitHub Copilot/Chat询问“如何使这段代码更易读和更易维护？”。
- 创建舞蹈和效果的视觉表示是可选的，但如果有时间建议实现。

### 任务摘要

1. 使用一个控制台应用显示输出。
1. 初始化森林的状态。
1. 每个生物为每个序列选择一个舞步。
1. 确定组合舞步对森林的魔法效果。
1. 更新每个序列后的森林状态。
1. 显示舞蹈完成后的森林最终状态。

### 入门提示

1. 如果你使用的是GitHub Codespace，你已经准备好了！
1. 如果你在本地运行，请确保已安装目标语言/框架。
    - [Node.js](https://nodejs.org)
    - [Python](https://www.python.org/downloads/)
    - [.NET](https://dot.net)
1. 创建一个文件夹存放你的代码。
    - JavaScript：创建一个名为`algora`的文件夹并添加一个名为`app.js`的文件。
    - Python：创建一个名为`algora`的文件夹并添加一个名为`app.py`的文件。
    - C#：创建一个名为`algora`的文件夹并执行`dotnet new console`。

### GitHub Copilot的提示

<a href="#">
    <img src="../../../Images/copilot-tips.jpg"  style="width: 830px" />
</a>

#### 使用Copilot提高效率
看看你能否使用Copilot发现代码的复杂度（BigO）。

1. 打开侧边栏中的[GitHub Copilot聊天视图](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat#asking-your-first-question)，确保解决方案文件仍然打开。

1. 向Copilot Chat询问代码的复杂度。

1. 让Copilot Chat使代码更高效。

1. 再次询问复杂度——是否有所改善？

#### 使用Copilot生成代码注释

1. 使用<kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>A</kbd>选中所有代码。

1. 按<kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>I</kbd>打开内联聊天。

1. 输入"/doc"

1. 请求Copilot Chat为函数添加注释。

#### 使用Copilot简化代码

1. 打开侧边栏的GitHub Copilot聊天。

1. 输入"/simplify"并按<kbd>Enter</kbd>。你也可以在"/simplify"后添加任何文本，给Copilot更多指示。

1. Copilot Chat建议了什么使代码更简单？

#### 有错误？

Copilot Chat也可以帮助解决错误！只需复制错误消息并粘贴到Chat中。通常这就是Copilot解决你问题所需的一切。