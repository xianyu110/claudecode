
---

## **轻松上手 AI 编程：15 分钟学会用 Claude Code 创作**

想用 AI 写代码，却总是被复杂的配置和环境搭建卡住？别担心！这篇文章将带你用 **Claude Code**，在短短 **15 分钟内**，从零开始做出你的第一个实用作品。即使你**完全不懂编程**，也能轻松掌握！

---

### **第一步：准备就绪——安装与配置**

在开始 AI 编程之旅前，我们首先需要做好一些基础准备。

#### **1.1 安装 Claude Code**

现在安装 Claude Code 变得**前所未有的简单**！我们强烈推荐**官方一键安装方式**，它能让你跳过 Node.js 的复杂配置，直达核心。

**💡 重要更新 (2025年12月1日)：** Claude Code 增加了地区检测。部分区域用户在执行安装命令时，可能需要配置命令行代理才能顺利执行。

**✅ 方案一：Claude Code 官方推荐方式（无需 Node.js）**

如果你选择以下推荐的安装方式，**无需提前安装 Node.js**。这大大简化了安装流程，避免了许多初学者常遇到的坑！

| 操作系统           | 步骤                                                                                        | 命令                                                                                  |             |
| :------------- | :---------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------- | ----------- |
| **Mac 用户**     | 1. 打开「终端」（Terminal）：在启动台中搜索即可找到。终端是使用命令与电脑交互的方式，你只需复制、粘贴并按回车。 <br> 2. **复制并粘贴以下命令，然后回车**： | ```bash<br>curl -fsSL [https://claude.ai/install.sh](https://claude.ai/install.sh)  | bash<br>``` |
| **Windows 用户** | 1. 点击开始菜单，搜索「PowerShell」。**右键选择「以管理员身份运行」**。 <br> 2. **复制并粘贴以下命令，然后回车**：                  | ```powershell<br>irm [https://claude.ai/install.ps1](https://claude.ai/install.ps1) | iex<br>```  |

安装过程通常需要 **1-2 分钟**，系统会自动下载所需组件。
**安装完成的标志**：你将看到提示信息 **「Claude Code installed successfully」**。

---

**✅ 方案二：Node.js 方案（传统安装方式）**

如果你对 Node.js 环境比较熟悉，或者因特定需求需要先安装 Node.js，也可以选择此方案。

1. **安装 Node.js**

   * 访问 [Node.js 官网](https://nodejs.org/zh-cn/download)。
   * **Mac 用户**：点击下载「macOS 安装程序(.pkg)」。
   * **Windows 用户**：点击下载「Windows 安装程序(.msi)」。如需更详细的教程，可参考 [此链接](https://blog.csdn.net/Little_Carter/article/details/155107677?fromshare=blogdetail&sharetype=blogdetail&sharerId=155107677&sharefrom=from_link&login=from_csdn)。

   **验证 Node.js 安装**：

   * **Mac 用户**：在 Finder「应用程序 -> 工具文件夹 -> 终端」中打开终端。
   * **Windows 用户**：按下 `Win + R` 键，输入 "cmd"，回车打开命令提示符。

   在终端或命令提示符中，输入并回车：

   ```plain
   node -v
   ```

   如果显示版本号，说明 Node.js 安装成功。
   接着输入并回车：

   ```plain
   npm -v
   ```

   如果显示版本号，说明 npm 也安装成功。
   ![Node.js和npm版本验证](https://ai.feishu.cn/space/api/box/stream/download/asynccode/?code=MzVmMjA4ZTNkOTIxNDBjZjNlYjdkZjMwOWM0ZGUzMzlfdTV5Nk9iZ3Z3bkhWRHZsdWVJTHJwOTl4elRSaHJhQnhfVG9rZW46QTRXdWJWZEl6b0tyQ0R4UHJvY2NmVHEzbmtkXzE3NjU5NDMwNDc6MTc2NTk0NjY0N19WNA)

2. **安装 Claude Code**
   无论你是 Windows 还是 Mac 用户，安装方式都相同。
   **复制以下内容，粘贴到终端或命令提示符，然后回车**：

   ```plain
   npm install -g @anthropic-ai/claude-code --registry=https://registry.npmmirror.com
   ```

   安装完成后，输入 `claude --version` 并回车。如果看到版本号，则说明 Claude Code 安装成功。
   ![Claude Code 版本验证](https://ai.feishu.cn/space/api/box/stream/download/asynccode/?code=YTgyNzA3Mzc1YjVlMWUxZmQzYjNhZDRmMzYyNWMzZjNfZTFYOXFRMDdpaU5DM1M2Y212bU82TzdqN3gyV1VQbVZfVG9rZW46QnNtbmI0RWxTb3pkWGh4RzRLamMwSUVZbnRkXzE3NjU5NDMwNDc6MTc2NTk0NjY0N19WNA)

---

#### **1.2 你需要一个 Claude 账号**

使用 Claude Code 的唯一**核心门槛**，是拥有一个可以在其内部调用的 Claude 账号。

你可以将 Claude Code 理解为一个**智能编程工具**，而大型语言模型（LLM）如 Claude 则是提供智能服务的**“后端大脑”**。就像你的手机可以选择不同的运营商，Claude Code 允许你接入不同的 LLM 服务，你只需要为使用的 LLM 付费。

由于 **Claude 官方通常会限制中国地区用户的直接访问和账号注册**，导致获取官方账号门槛较高。因此，我们**强烈推荐使用中转方案**。

**中转方案优势**：你的请求会先发送到中转服务商，再由服务商请求 Claude 官方。这样可以**避免封号、无需科学上网**等问题。

| 方案类型     | 名称                            | 链接                                                                     | 备注           |
| :------- | :---------------------------- | :--------------------------------------------------------------------- | :----------- |
| **中转服务** | **GACcode**                   | [https://maynorai.tqfk.xyz/item/17](https://maynorai.tqfk.xyz/item/17) | 追求最佳效果和稳定性推荐 |
| **中转服务** | **ClaudeCodeCodexGemini 一个月** | [https://maynorai.tqfk.xyz/item/7](https://maynorai.tqfk.xyz/item/7)   | 经济实惠的月度选择    |

**详细安装教程**：
关于账号的详细配置，可以参考这篇 [Claude Code 使用教程](https://ai.feishu.cn/wiki/CVPBwfMFmis0r9k60vaclVArnHn?from=space_home_recent&pre_pathname=/drive/home/&previous_navigation_time=1765942709298)。

---

#### **1.3 降低上手门槛：安装 Claude Code for VS Code 插件**

对于不习惯使用终端或命令行的朋友来说，拥有一个**图形界面**至关重要！Claude Code 官方提供了强大的 VS Code 插件，让你能在更友好的环境中进行 AI 编程。

**第一步：安装 VS Code**
访问 [VS Code 官网](https://code.visualstudio.com/) 下载并安装这款免费且强大的代码编辑器。

**第二步：安装 Claude Code 插件**
你可以通过以下两种方式安装插件：

1. **点击链接**：[https://marketplace.visualstudio.com/items?itemName=anthropic.claude-code](https://marketplace.visualstudio.com/items?itemName=anthropic.claude-code)，会自动跳转到 VS Code 并提示安装。
2. **在 VS Code 插件市场搜索**：「Claude Code」并点击安装。
   ![VS Code 插件市场搜索](https://ai.feishu.cn/space/api/box/stream/download/asynccode/?code=ZmE2ZTI3MTY0YWExZDA2M2I4MTJlMmYxZGNlNjAyZWRfQnQ4NWNhNDlNMGFLR2h2cldQQjJKRUREMTk2b3ZFc05fVG9rZW46SjlzU2JYMmN2b3hTUk14N2hPOWNtMnRQbkxjXzE3NjU5NDMwNDc6MTc2NTk0NjY0N19WNA)

**如何使用插件**
安装完成后，点击 VS Code 侧边栏的 **Claude Code 图标**即可开始使用。
![Claude Code 插件界面](https://ai.feishu.cn/space/api/box/stream/download/asynccode/?code=YTAyNTJlOTVhMTM5NGUxNGE2ZjhhNjcyOTg4MjYwOTdfWlBTb2gwQUFZaWpLYjNUYklsUkVPSkZxNFl0T1JmVmpfVG9rZW46U0pSSGJlc3E4b2p6NDd4SmlCNGNOY1lTbmxoXzE3NjU5NDMwNDc6MTc2NTk0NjY0N19WNA)

**简化 API 配置：使用 cc Switch**
配置 `base url` 和 `API key` 可能会比较繁琐。推荐使用 **`cc Switch` 工具**（[链接](https://waytoagi.feishu.cn/wiki/WZZRwjxAbiNow5ki0s6clQNLnsb#share-HJv3dKW7Co1mMcx1tp4cNA75nme)）来简化这一过程：

* 在 `cc Switch` 中**勾选「应用到 Claude code 插件」**。
* **重新启动 VS Code**，配置即可生效。
  ![cc Switch 配置截图1](https://ai.feishu.cn/space/api/box/stream/download/asynccode/?code=ZDgyOWY4ZGFmNjlkNjQwODI5N2IxNmYyYjFlZjllMmNfTDZtVnQ5RGY3cEFiNENkaTNVSG9HZnkyUXJORmxvMnhfVG9rZW46RE4zTGJYOGZ5b295UGN4OGp5amNzdldXbjdjXzE3NjU5NDMwNDc6MTc2NTk0NjY0N19WNA)
  ![cc Switch 配置截图2](https://ai.feishu.cn/space/api/box/stream/download/asynccode/?code=ZjdmMTFkYTc0OTFmMDk2NmFlMDlkNDNjOTdlNDZhZmVfSlpNTjR4dDB0c1RiM0tWOU5sNzNJeVZ1QllRSTlzZnVfVG9rZW46UE1POGJ2M1lMb0VYNlJ4N2VQRWM2S0pzblNmXzE3NjU5NDMwNDc6MTc2NTk0NjY0N19WNA)

**开启 Claude Code 全自动模式**
默认情况下，Claude Code 提供「plan（规划）」、「手动确认」和「自动编辑」模式。要实现**完全自动化**的编程体验，你可以在 cc 插件中开启 **「Allow Dangerously Skip Permissions」** 选项。这将允许 Claude Code **自动运行命令，无需二次确认**，大大提高效率。你也可以将全自动模式配置为默认模式。
![开启全自动模式](https://ai.feishu.cn/space/api/box/stream/download/asynccode/?code=MWFhZjE3ZDc5OTg4NTEzY2M2MDEyOGMxNTI2OTJmNmJfMVBoVmg4aWZ3bnAyWVZKTUZicHdkelNCTEkxNllZTHhfVG9rZW46VGUwV2J2Slc4b2dhemx4VWhOUWNaVXpwblZlXzE3NjU5NDMwNDc6MTc2NTk0NjY0N19WNA)

---

### **第二步：创作你的第一个作品——待办清单**

现在，一切准备就绪，让我们用 Claude Code 亲手制作一个实用的小工具！

#### **2.1 我们要做什么？**

我强烈建议你的第一个项目是制作一个**「待办清单网页」**。
**选择它的理由**：

* **够简单**：15 分钟内即可完成。
* **够实用**：做完后真的能用，即时获得成就感。
* **够完整**：麻雀虽小，五脏俱全，包含增、删、改、查等核心功能。

**最终效果预览**：
你将得到一个简洁美观的网页，能够：

* **添加任务**：输入框 + 添加按钮。
* **标记完成**：点击任务，任务文字自动划线。
* **删除任务**：每个任务旁有独立的删除按钮。
* **界面设计**：简洁美观，符合现代审美。

#### **2.2 创建项目文件夹**

回到你之前打开的终端（或命令提示符），输入以下命令并回车：

```bash
mkdir my-todo-app
cd my-todo-app
claude
```

**命令解释**：

* `mkdir my-todo-app`：**创建一个名为「my-todo-app」的文件夹**，用于存放你的项目文件。
* `cd my-todo-app`：**进入这个新建的文件夹**。
* `claude`：**启动 Claude Code**，现在你将进入与 AI 对话的模式。

#### **2.3 最重要的一步：先规划再动手**

直接让 AI 编写代码很容易导致混乱。**聪明的做法是，首先让 AI 给你一个详细的实现计划**。这样你就能清楚地了解要做的内容、技术栈和大致步骤，确认无误后再开始实际的代码编写。

**复制这段话，发送给 Claude**：

```plain
我想做一个待办清单网页，要求：
1. 可以添加新任务（输入框+添加按钮）
2. 可以点击任务标记为完成（会有划线效果）
3. 可以删除任务（每个任务旁边有删除按钮）
4. 界面要简洁美观，用现代化的设计

请先给我一个实现计划，包括用什么技术、分几个文件、大概的实现步骤，等我确认后再开始写代码。
```

**Claude 会回复类似这样的计划**：

```plain
好的，我来规划这个待办清单应用：

## 技术选择
- HTML：页面结构
- CSS：样式设计（使用 Flexbox 布局）
- JavaScript：交互逻辑

## 文件结构
1. index.html - 主页面
2. style.css - 样式文件
3. script.js - 功能代码

## 实现步骤
1. 创建 HTML 基础结构（输入框、按钮、任务列表区域）
2. 编写 CSS 样式（现代卡片设计+渐变背景）
3. 实现 JavaScript 功能（添加、完成、删除）
4. 添加本地存储，刷新页面后数据不丢失

准备好了吗？我可以开始实现。
```

**你只需要回复**：「**好的，开始吧**」。

#### **2.4 看着代码自己写出来**

这绝对是整个过程中**最神奇、最令人兴奋**的部分！

你会看到 Claude 开始自动工作：

* **创建 `index.html` 文件**，并写入页面基础结构。
* **创建 `style.css` 文件**，并编写所有样式代码。
* **创建 `script.js` 文件**，并实现所有交互逻辑。

整个过程你**无需做任何事**，就像看着一位资深程序员在你的电脑上高效工作。
每创建一个文件，Claude 都会实时告诉你它正在做什么，例如：

```plain
创建 index.html...
添加了页面基础结构，包括标题、输入区域和任务列表容器

创建 style.css...
使用了现代化的卡片设计，添加了渐变背景和阴影效果

创建 script.js...
实现了添加、完成、删除功能，并加入了本地存储
```

大概 **2-3 分钟**，所有代码就会全部写完。

#### **2.5 打开浏览器看效果**

代码编写完成后，Claude 会告诉你如何运行查看效果。通常它会提示：

```plain
已完成！你可以直接用浏览器打开 index.html 查看效果。

或者在终端运行：
python3 -m http.server 8000

然后在浏览器访问 http://localhost:8000
```

**查看方式**：

* **Mac 用户**：直接在 Finder 中找到 `my-todo-app` 文件夹，**双击 `index.html`** 文件。
* **Windows 用户**：在文件资源管理器中找到 `my-todo-app` 文件夹，**双击 `index.html`** 文件。

你的浏览器会立即打开，你将看到一个：

* 顶部大标题「我的待办清单」。
* 一个输入框和旁边的「添加」按钮。
* 下方是任务列表区域。

**现在，尝试添加你的第一个任务**：「**学会用 Claude Code**」，然后点击添加。
恭喜你！你的第一个任务出现了！你可以点击任务来**标记完成**（它会划线），旁边的小按钮则可以**删除**它。

**🎉 恭喜！这就是你用 AI 独立完成的第一个作品！**

---

### **第三步：加一个新功能——迭代优化**

现在你可能想，「我能不能修改一下，或者加点新功能？」当然可以！这正是 AI 编程的强大之处——**迭代和修改超级简单**。

#### **3.1 提一个新需求**

假设你想给每个任务加上创建时间，让它显示在任务文字下方，并且用小号灰色字体呈现。
**直接在 Claude Code 的对话中输入**：

```plain
我想给每个任务加上创建时间，格式是「2025-11-10 15:30」，显示在任务文字的下面，用小字灰色显示
```

#### **3.2 Claude 会自动修改**

Claude 接收到你的需求后，会：

1. **告诉你需要修改哪些地方**（通常是 `script.js` 和 `style.css`）。
2. **自动修改 `script.js`**，添加记录和显示时间戳的逻辑。
3. **自动修改 `style.css`**，为时间戳添加小字灰色的样式。

**你只需要刷新浏览器**，新功能就会立即生效！

这就是**AI 协作**的真实体验：你提出需求，AI 编写代码，你验收效果。不满意？继续对话调整，直到完全符合你的预期。

#### **3.3 试试其他功能**

你可以尝试提出更多有趣的需求，看看 Claude 如何帮你实现：

* 「**加一个优先级标签，重要的任务显示红色**」
* 「**加一个全部删除按钮**」
* 「**换一个配色方案，我想要蓝色系**」
  每次，Claude 都会理解你的意思，并自动修改代码以满足你的需求。

---

### **第四步：新手常见问题解答**

在指导众多学习者使用 Claude Code 的过程中，我总结了一些新手最常遇到的问题。

#### **Q1：改错了怎么办？**

**别慌！Claude Code 拥有「时光机」功能，让你轻松回退。**

* **方法一：按 `ESC` 两次**：这是最快捷的方式，可以立即回退到上一个版本。
* **方法二：输入命令**：

  ```plain
  /rewind
  ```

  Claude 会列出所有历史版本，你可以选择回到任何一个时间点。
* **方法三：直接说**：「**刚才那个改动我不喜欢，还原回去**」。Claude 会理解并执行。

#### **Q2：我完全不懂代码，怎么知道 Claude 做的对不对？**

答案很简单：**你不需要懂代码，你只需要测试功能**。
这就像你不需要懂汽车发动机的原理，也能知道车能不能开一样。

* **添加任务**试试，能加上吗？
* **标记完成**试试，有划线吗？
* **删除**试试，真的删掉了吗？
* **刷新页面**，数据还在吗？

只要**功能表现正确，代码就是对的**。如果发现问题，直接告诉 Claude：「**删除按钮点了没反应**」，它会自己检查并修复。

#### **Q3：为什么有些教程说要装 Node.js？**

这是一个很好的问题，说明你正在积极思考。
**简单回答**：如果你使用的是我这篇教程**推荐的「官方一键安装方式」（curl 或 PowerShell 命令）**，那么你就**不需要安装 Node.js**。
**完整解释**：Claude Code 有多种安装方式。如果通过 `NPM` 包管理器安装（命令如 `npm install -g @anthropic-ai/claude-code`），则确实需要预先安装 Node.js，因为 `NPM` 是 Node.js 的包管理器。但是，官方的一键安装脚本已经**将所有依赖都打包好了**，无需你手动配置 Node.js 环境，即装即用。
**对新手来说**：**跟着本教程的步骤走，避免使用 `NPM` 安装方式，就不会遇到 Node.js 的问题**。

#### **Q4：我应该从这个开始学编程吗？**

这取决于你的学习目标。

* **如果你想快速做出东西**（例如制作一个小工具、验证一个想法、自动化工作流程）：

  * **从 Claude Code 开始是绝对正确的选择**。
  * 边做边学，遇到问题就**直接向 Claude 提问**。
  * 遇到不理解的概念，让 Claude 帮你解释。
* **如果你想成为专业的软件开发者**：

  * Claude Code 是一个**极佳的辅助工具**，但不能完全替代系统的学习。
  * 推荐的学习路径是：**先用 AI 做出第一个项目（建立信心）** → **系统学习基础知识**（如 CS50 课程、FreeCodeCamp） → **再利用 AI 加速开发和学习**。


---

### **下一步：你可以做什么？**

完成了这 15 分钟的教程，你已经成功掌握了：

* ✅ **安装和配置 Claude Code**
* ✅ **先规划再动手的 AI 编程方法论**
* ✅ **让 AI 自动编写代码并运行**
* ✅ **向 AI 提出需求并进行功能迭代修改**
* ✅ **解决新手常见问题**

接下来，我鼓励你尝试以下挑战：

1. **做个你真正需要的工具**：

   * 一个简单的记账页面？
   * 一个个性化的倒计时器？
   * 一个展示你个人技能的简历网站？
2. **挑战：给待办清单加更多功能**：

   * 增加一个「优先级」分类（高/中/低）？
   * 添加一个任务搜索功能？
   * 把页面配色方案换成你最喜欢的颜色？
3. **加入社区，分享和交流**：


   * 把你的作品分享出来，让我们一起交流和进步！

---

### **最后说两句**

那个 11 岁的小女孩在用 Claude Code 完成作品后，兴奋地跟我说：「**原来编程没那么难，就像跟一个很厉害的朋友聊天**。」她说的完全正确。

2025 年的 AI 编程工具，其核心价值在于**极大地降低了「想法」到「实现」的门槛**。
过去，你可能需要花费数月时间学习代码基础才能做出一个像样的东西；而现在，你可以**先做出东西，再慢慢理解背后的原理**。

这并不是说传统的系统学习不再重要，而是**学习的路径和顺序发生了根本性变化**。先用 AI 亲手做出第一个作品，建立起信心和兴趣，然后再去系统地学习底层知识和理论，这种方式反而让更多人能够坚持下来，真正爱上编程。

所以，请不要再担心自己「不会编程」。
**立刻打开 Claude Code，用 15 分钟试一试，你可能会发现一个全新的世界！**

---

### **快速参考：Claude Code 常用命令**

这里汇总了一些你在 Claude Code 中可能经常使用的命令，方便你查阅。

| 命令                   | 功能                        |
| :------------------- | :------------------------ |
| `claude`             | **启动 Claude Code**，进入对话模式 |
| `mkdir project-name` | **创建新项目文件夹**              |
| `cd project-name`    | **进入项目文件夹**               |
| `/help`              | **查看所有帮助信息**              |
| `/rewind`            | **回退到历史版本**（「时光机」功能）      |
| `/clear`             | **清空当前对话记录**              |
| `/exit`              | **退出 Claude Code**        |

---

### **推荐提示词模板**

当你开始一个新的项目时，可以使用以下模板来与 Claude 进行高效的沟通和规划：

```plain
做一个[项目类型]，需要：
1. [功能1]
2. [功能2]
3. [功能3]
界面要[风格要求]

请先给我一个实现计划，等我确认后再开始写代码。
```
