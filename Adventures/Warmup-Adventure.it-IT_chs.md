## GitHub Copilot 热身冒险

<a href="#">
    <img src="../Images/warm-up.jpg" style="width: 830px" />
</a>

GitHub Copilot 是一个基于 AI 的工具，可以帮助你写出更好的代码。在这次热身冒险中，你将有机会了解并尝试使用 Copilot。以下是一些你可以用 GitHub Copilot 做的事情：

- 将评论转换为代码。需要进行 HTTP 调用、过滤数组或执行其他任务吗？写一个评论，Copilot 会将其转换为代码。
- 创建用户界面。使用纯 HTML/CSS/JavaScript 或你选择的库/框架。
- 创建 SQL 查询。
- 创建单元测试。
- 用新的编程语言写代码。
- 解释你正在编写的代码。
- 以及更多！

如果你对 GitHub Copilot 完全陌生，请观看此视频了解它可以如何改善你的开发工作流程。观看完视频后，回到这里选择一个冒险开始。

[![GitHub Copilot 视频](../Images/copilot-video.png)](https://www.youtube.com/watch?v=Dlt-DCLHnxM)

## 开始：安装 GitHub Copilot 扩展

按照以下步骤在 Visual Studio 或 Visual Studio Code 中安装 GitHub Copilot 扩展。

1. 如果尚未安装，请安装 [Visual Studio](https://visualstudio.microsoft.com/) 或 [Visual Studio Code](https://code.visualstudio.com/)。

1. 按照 https://docs.github.com/en/copilot/getting-started-with-github-copilot 上的步骤安装 GitHub Copilot。

## 如果我没有 GitHub Copilot 许可证怎么办？

**你是学生吗？** 了解更多关于如何 [配置和访问 GitHub Copilot](https://techcommunity.microsoft.com/t5/educator-developer-blog/step-by-step-setting-up-github-student-and-github-copilot-as-an/ba-p/3736279)。

如果你目前没有 GitHub Copilot 许可证，你可以：

- [注册免费试用](https://github.com/login?return_to=%2fgithub-copilot%2fsignup)。
<!-- - 如果你有优惠券代码，<a href="../README.it-IT.md#coupon">查看如何使用。</a>。 -->

## 你的第一个冒险：回声之室

让我们从你的第一个冒险开始！

<a href="#">
    <img src="../Images/echo-castle.jpg" style="width: 830px" />
</a>

### 背景：

在最高的山丘上，俯瞰王国，矗立着雄伟的 Echo 城堡。在它的石墙内，有一个被称为“回声之室”的房间。这个房间与其他任何房间都不同，它有神秘的力量，可以对进入房间的任何人进行回声。然而，回声之室并不对任何数字进行回声；它总是对序列中的下一个数字进行回声。

传说中，一位巫师给这个房间施了魔法，以测试访问者的智慧。房间会对序列中的数字进行回声，只有那些能够预见下一个回声的人才被认为值得城堡中的隐藏宝藏。

### 目标：

你的任务是进入回声之室，听取它的序列，然后预测下一个数字的回声。你被提供了一系列过去房间中的回声数字。使用这些数字来确定序列中的下一个数字。

### 规格：

1. **输入**:
    - 一个至少包含三个数字的序列列表。这个列表代表过去房间中的回声数字。
    
2. **输出**:
    - 一个代表序列中下一个数字的单一数字。

3. **假设**:
    - 序列总是算术级数（连续数字之间的差异是固定的）。

### 示例数据：

考虑序列: [3, 6, 9, 12]

房间中下一个回声的数字应该是: 15

### 约束：

- 以下解决方案使用 JavaScript 和 Node.js，但如果你愿意，也可以使用 Copilot 用其他语言写代码。

### 高级任务摘要：

1. 使用控制台应用程序显示输出。
1. 创建一个常量来保存提供的数字序列。
1. 确定连续数字之间的共同差异。
1. 使用识别的模式预测序列中的下一个数字。

### GitHub Copilot 步骤

此解决方案使用 JavaScript 和 [Node.js](https://nodejs.org)。如果你愿意，可以使用其他语言/框架。

1. 在选择的文件夹中创建一个名为 `echo-chamber.js` 的文件。

1. 在文件中添加一个名为 `echoes` 的 `const` 来保存数字序列：

    ```js
    const echoes = [3, 6, 9, 12];
    ```

1. 在 `echoes` 常量之后键入以下代码。Copilot 应该会建议一些代码来帮助你确定序列中连续数字之间的差异。

    ```js
    function predictNext(echoes) {
    ```

1. 按 <kbd>Tab</kbd> 接受建议。应添加以下函数体。注意，你可能会看到不同的代码建议。

    ```js
    function predictNext(echoes) {
        let difference = echoes[1] - echoes[0];
        let next = echoes[echoes.length - 1] + difference;
        return next;
    } 
    ```

1. 在函数之后插入新行，Copilot 应该会建议如下代码。如果没有，开始键入 `console.log`。按 <kbd>Tab</kbd> 接受建议。

    ```js
    console.log(predictNext(echoes));
    ```

1. 将光标移到 `predictNext` 函数上方并选择 <kbd>CTRL + i</kbd>（Windows）或 <kbd>CMD + i</kbd>（Mac）。

1. 在出现的文本框中输入 `/doc` 并按 <kbd>Enter</kbd>。你应该会看到为函数生成的注释。

    ![在 VS Code 中的内联聊天](../Images/inline-chat.png)

1. 选择 `接受` 以接受建议。

1. 你应该会看到为函数生成注释。

    **注意：** 除了生成文档，你还可以使用注释生成代码。

1. 现在假设你想存储房间中先前回声的“记忆”数字。在 `echoes` 变量之后添加如下代码。

    ```js
    const memories = [];
    ```

1. 在 `predictNext` 函数中 `return next` 语句 **上方** 添加以下注释并按 <kbd>Enter</kbd>。按 <kbd>Tab</kbd> 接受建议。

    ```js
    // 存储整个序列包括预测的数字到 memories
    ```

1. 你应该会看到类似如下生成的代码：

    ```js
    memories.push(...echoes, next);
    ```

1. 保存 `echo-chamber.js` 文件并在创建文件的文件夹中打开一个终端窗口。

1. 运行以下命令以执行代码。这假设你已经安装了 [Node.js](https://nodejs.org)。

    ```bash
    node echo-chamber.js
    ```

1. 你应该会在控制台上看到 `15`，这是序列中的下一个数字。

1. 添加注释，看看你是否可以让 Copilot 为你打印出记忆到控制台。

## Echo 城堡的隐藏宝藏现在属于你！

<a href="#">
    <img src="../Images/echo-castle-treasure.jpg" style="width: 830px" />
</a>

你已经完成了 GitHub Copilot 的第一个“热身”冒险！查看 [Adventures](../Adventures) 文件夹中其他的冒险，看看 GitHub Copilot 可以用于的其他方式。