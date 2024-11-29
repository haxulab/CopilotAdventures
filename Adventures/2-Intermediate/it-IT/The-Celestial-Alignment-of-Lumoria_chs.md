## Lumoria的天体对齐

<a href="#">
    <img src="../../../Images/lumoria.jpg" style="width: 830px" />
</a>

### 背景

在广阔的Galaxia星云中，Lumoria星系即将发生一个罕见的现象。围绕Lumoria太阳运行的行星会以一场几千年才会发生一次的天体舞蹈形式对齐。这种对齐对Lumoria太阳光到达每个行星的方式有独特的影响。

### 目标

你的任务是计算在这次对齐过程中每个行星收到的光强度。根据行星与Lumoria太阳之间的距离及其相对位置，确定哪些行星可能会因其他行星投下的阴影而经历光强度的减弱。

### 规格

1. **行星数据：**

| 行星名称       | 距离(天文单位) | 尺寸(公里)  |
| -------------- | -------------- | ----------- |
| Mercuria       | 0.4            | 4879        |
| Earthia        | 1              | 12742       |
| Marsia         | 1.5            | 6779        |
| Venusia        | 0.7            | 12104       |

行星没有按照它们距离Lumoria太阳的距离排序，因此需要你来处理这一点。

2. **光的动态：**

- 如果一个小行星在大行星后面（相对于Lumoria太阳），它会处于阴影之中，不会受到光照（`无`）。
- 如果一个大行星在小行星后面（相对于Lumoria太阳），它会受到`部分`光照。
- 如果一个行星被多个行星的阴影覆盖，它将被标记为`无（多重阴影）`。
- 如果两个行星大小相似并且在对齐中靠近彼此，它们可能会部分遮挡彼此，但为简单起见，你可以认为它们都受到完全光照。

3. **输出：**
   - 你的系统应该生成一个行星和它们接收到的光强度的列表：`完全`、`部分`、`无`或`无（多重阴影）`。

### 限制

- 使用GitHub Copilot，并用你喜欢的任意语言编写模拟代码。
- 集中于清晰简洁的代码，并有效地管理行星的检查。通过询问GitHub Copilot/Chat："如何使这段代码更易读和可维护？"
- 如果有时间，可以创建行星的SVG视觉表示图，但这不是必需的。

### 高级任务摘要

1. 使用控制台应用程序显示输出。
2. 根据它们距离Lumoria太阳的距离对行星列表进行排序。
3. 遍历排序后的行星列表。
4. 对于每个行星，检查距离Lumoria太阳更近的行星，看看它们是否投下阴影在其他行星上。
5. 显示每个行星接收到的光强度。

### 入门提示

1. 如果你正在使用GitHub Codespace，那你已经准备好了！
2. 如果你在本地运行，请确保已安装目标语言/框架。
   - [Node.js](https://nodejs.org)
   - [Python](https://www.python.org/downloads/)
   - [.NET](https://dot.net)
3. 创建一个文件夹来存放你的代码。
   - JavaScript: 创建一个名为`lumoria`的文件夹，并添加一个名为`app.js`的文件。
   - Python: 创建一个名为`lumoria`的文件夹，并添加一个名为`app.py`的文件。
   - C#: 创建一个名为`lumoria`的文件夹，并运行`dotnet new console`。

### GitHub Copilot 提示

<a href="#">
    <img src="../../../Images/copilot-tips.jpg"  style="width: 830px" />
</a>

首先，你需要将行星放入一个你可以操作的数据结构中。

1. 复制以前显示的Markdown表格。
2. 打开[GitHub Copilot Chat视图](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat#asking-your-first-question)，并输入以下文本。用你选择的语言替换"JavaScript"。

   ```text
   将此Markdown列表转换为JavaScript对象数组
   ```
3. 在你的评论下粘贴Markdown表格并按下回车键。
4. 将生成的行星数组插入到你的代码中。

```js
// 光强度数组

// 遍历排序后的数组

    // 创建一个对象以跟踪比当前行星更接近太阳的较大和较小行星的数量

    // 对于行星数组中当前行星前面的所有行星，如果它们比当前行星大则增加Larger，如果它们比当前行星小则增加Smaller

    // 如果count.larger === 0且count.smaller === 0，添加行星名称并将"完全"推送到lightIntensity中

    // 如果count.smaller > 0且count.larger === 0，添加行星名称并将"部分"推送到lightIntensity中

    // 如果count.larger === 1，添加行星名称并将"无"推送到lightIntensity中

    // 如果count.larger > 1，添加行星名称并将"无（多重阴影）"推送到lightIntensity中

// 打印lightIntensity数组
```

#### 使用 Copilot 提高效率

看看是否可以使用 Copilot 来发现代码的复杂度（BigO表示法）。

1. 打开 GitHub Copilot Chat 视图（如果尚未打开）。确保解决方案文件仍然打开。
2. 询问 Copilot Chat 代码的复杂性。
3. 询问 Copilot Chat 使代码更高效。
4. 再次询问复杂度是否有所改善？

#### 使用 Copilot 生成代码注释

1. 使用 <kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>A</kbd> 高亮所有代码。
2. 按 <kbd>Ctrl</kbd>/<kbd>Cmd</kbd>+<kbd>I</kbd> 打开内联聊天。
3. 输入 "/doc"。
4. 询问 Copilot Chat 文档注释功能。

#### 使用 Copilot 简化你的代码

1. 打开 GitHub Copilot Chat 在侧边栏。
2. 输入 "/simplify" 并按下 <kbd>Enter</kbd>。你也可以在 "/simplify" 后添加任何文本来给 Copilot 更多的指示。
3. Copilot Chat 提出的简化建议是什么？

#### 有错误？

Copilot Chat 也可以帮助解决错误！只需复制错误信息并粘贴进聊天窗口。大多数情况下，这就足以让 Copilot 帮助你解决问题。