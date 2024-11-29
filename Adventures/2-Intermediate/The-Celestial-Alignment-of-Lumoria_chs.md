排列

![Lumoria](../../Images/lumoria.jpg)

### 背景

在浩瀚的Galaxia星云中，Lumoria恒星系统即将发生一种罕见的现象。围绕Lumoria太阳旋转的行星们正在进行一次几千年才出现一次的天体排列。这种排列对Lumoria太阳发出的光到达每颗行星的方式有着独特的影响。

### 目标

你的任务是计算每颗行星在这一排列期间所接收到的光线强度。根据行星与Lumoria太阳的距离及其相对位置，确定哪些行星可能由于其他行星的遮挡而经历光强度的下降。

### 规格

1. **行星数据:**

| 行星名称 | 距离（天文单位） | 大小（公里） |
|---------|-----------------|-------------|
| Mercuria | 0.4             | 4879       |
| Earthia  | 1               | 12742      |
| Marsia   | 1.5             | 6779       |
| Venusia  | 0.7             | 12104      |

这些行星没有按照它们到Lumoria太阳的距离排序，所以你需要处理这个问题。

2. **光动态:**
- 如果一颗小的行星在一颗大的行星后面（相对于Lumoria太阳），它将处于阴影中并且不会接收到光（`None`）。
- 如果一颗大的行星在一颗小的行星后面（相对于Lumoria太阳），它将接收到“部分”光（`Partial`）。
- 如果一颗行星处于多颗行星的阴影中，它将被标记为`None (Multiple Shadows)`。
- 如果两颗行星大小相似并且在排列中接近，它们可能会部分遮挡彼此，但为了简化，可以认为它们都接收到满光（`Full`）。

3. **输出:**
    - 你的系统应输出行星及其接收到的光强度列表：`Full`, `Partial`, `None`或`None (Multiple Shadows)`。

### 约束

- 使用GitHub Copilot，并用你喜欢的任何语言编写模拟程序。
- 重点编写清晰简洁的代码，能有效地处理行星检查。向GitHub Copilot/Chat询问：“如何使这段代码更具可读性和可维护性？”。
- 如果有时间，鼓励创建一个行星的SVG视觉表示，但这不是必需的。

### 高级任务概要

1. 使用控制台应用程序输出结果。
2. 根据到Lumoria太阳的距离排序行星列表。
3. 遍历排序后的行星列表。
4. 对于每颗行星，检查离Lumoria太阳较近的行星是否会对其他行星投下阴影。
5. 输出每颗行星接收到的光照强度。

### 入门提示

1. 如果你使用的是GitHub Codespace，你已经准备好了！
2. 如果在本地运行，确保你安装了目标语言/框架。
    - [Node.js](https://nodejs.org)
    - [Python](https://www.python.org/downloads/)
    - [.NET](https://dot.net)
3. 创建一个代码文件夹。
    - JavaScript: 创建一个名为 `lumoria` 的文件夹，并添加一个名为 `app.js` 的文件。
    - Python: 创建一个名为 `lumoria` 的文件夹，并添加一个名为 `app.py` 的文件。
    - C#: 创建一个名为 `lumoria` 的文件夹，并运行 `dotnet new console`。

### GitHub Copilot 提示

[![Copilot Tips](../../Images/copilot-tips.jpg)](#)

首先，你需要将行星数据放入一个你可以使用的数据结构中。

1. 复制之前展示的Markdown表格。
2. 打开 [GitHub Copilot Chat视图](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat#asking-your-first-question) 并输入以下文本。将你的语言选择替换为“JavaScript”。
    
    ```text
    turn this markdown list into a JavaScript array of objects
    ```

3. 在评论下方粘贴Markdown表格并按下回车键。
4. 将生成的行星数组插入到代码中。

```js
// light intensity array

// traverse the sorted array

    // create an object to track the count of Larger and Smaller planets that are closer to the sun than the current planet

    // for all the planets that come before this planet in the planets array, increment Larger if they are larger than the current planet or Smaller if they are smaller than the current planet

    // if count.larger === 0 and count.smaller === 0 push planet name and "Full" to lightIntensity 

    // if count.smaller > 0 and count.larger === 0 push planet name and "Partial" to lightIntensity

    // if count.larger === 1 push planet name and "None" to lightIntensity

    // if count.larger > 1 push planet name and "None (Multiple Shadows)" to lightIntensity

// print the lightIntensity array
```

#### 使用Copilot提高效率

看看你能否使用Copilot找出代码的复杂度（BigO符号）。

1. 打开侧边栏中的 [GitHub Copilot Chat视图](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat#asking-your-first-question)。确保你仍然打开了解决方案文件。

1. 询问Copilot Chat代码的复杂度是什么。

1. 询问Copilot Chat如何使代码更高效。

1. 再次询问复杂度——是不是更好了？

#### 使用Copilot生成代码注释

1. 使用<kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>A</kbd>突出显示所有代码。

1. 按下<kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>I</kbd>打开内联聊天。

1. 输入`/doc`

1. 让Copilot Chat为函数生成文档。

#### 使用Copilot简化代码

1. 打开侧边栏中的GitHub Copilot Chat。

1. 输入`/simplify`并按下回车键。你也可以在“/simplify”后添加任何文本，以便给Copilot更多的指示。

1. Copilot Chat建议你做些什么来简化代码？

#### 出现错误？

Copilot Chat也可以帮助你解决这些问题！只需要复制错误信息并粘贴到Chat中。通常这就是Copilot解决问题所需要的一切。