---
layout: center
class: text-center
---

# 第四章：CLI Agent
## 脱离图形界面，走向"全量自动化"

<div class="mt-8 opacity-50">
  <lucide-terminal class="text-6xl mx-auto text-green-400" />
</div>

---
layout: default
---

# <lucide-bot class="inline-block mr-2 mb-1 opacity-70"/>为什么我们需要命令行 AI？

IDE AI 是"驾驶辅助"，受到屏幕与人为焦点的限制；而在服务器后台运作的 CLI Agent 则是真正的"无人驾驶"，适合批处理与流水线。

<div class="grid grid-cols-2 gap-8 my-10">

  <div class="bg-gray-900 border border-slate-700 p-5 rounded-lg font-mono">
    <div class="text-xs text-slate-500 mb-2"># 典型 CLI Agent: Claude Code</div>
    <div class="text-green-400">$ claude "在这个项目里找出所有的 TODO 注释，解决它们并生成 git commit!"</div>
    <div class="mt-4 text-xs text-slate-400">
      -> 搜索文件...<br/>
      -> 修改 5 个文件...<br/>
      -> 运行 eslint...<br/>
      -> git commit -m "Fix TODOs"<br/>
    </div>
  </div>

  <div class="flex flex-col justify-center space-y-4 text-sm opacity-90 leading-relaxed pl-4 border-l border-slate-700">
    <p><strong class="text-green-300">✅ 可管道化：</strong> <br/>`cat data.csv | claude "精简成 json"`，融入传统的 unix 脚本。</p>
    <p><strong class="text-green-300">✅ 可后台无人值守：</strong> <br/>挂在服务器跑整夜的数据处理任务。</p>
    <p><strong class="text-green-300">✅ 极低资源消耗：</strong> <br/>不需要打开笨重的 IDE，远程 SSH 一样跑。</p>
  </div>
</div>

<!--
去掉 UI 是必经之路，一个软件好用是因为有好 UI，方便人类使用，但是再进一步，不需要人类也能自动执行任务的软件是更好用的软件。
-->

---
layout: two-cols
---

# <lucide-file-text class="inline-block mr-2 mb-1 opacity-70"/>Skill 机制：对抗系统熵增

> AI Agent 的"SOP 规范标准"

虽然我们可以让 Agent 放开手脚干活，但它不懂物理世界的**隐性规矩**。这就是预设 Skill 文档的价值。

<div class="pr-6 mt-4">
  <div class="bg-blue-900/10 p-5 rounded-lg border border-blue-500/30">
    <h3 class="text-blue-300 text-sm font-bold mb-3 flex items-center gap-2"><lucide-file-signature class="w-4 h-4"/> 什么是 Skill？</h3>
    <ul class="text-sm opacity-80 list-disc pl-5 space-y-2">
      <li>显式的、人类可读的 Markdown 策略指导。</li>
      <li>Agent 进入任何新项目的 <b>Initialization (初始化) 通关必读</b>。</li>
      <li>将团队的"隐藏共识"与"安全红线"硬编码到上下文。</li>
    </ul>
  </div>
</div>

::right::

<div class="h-full flex items-center bg-slate-900 mt-14 p-4 rounded-xl border border-slate-700 shadow-xl overflow-hidden font-mono text-xs">
```markdown
# Skill: 实验室 CSV 分析规范

## 步骤
1. 必须优先调用 `head -n 5` 观察字段。
2. 缺失值统一使用 0 填充。
3. 必须输出箱线图的 python 代码并在本地执行。

## 约束 (CRITICAL)
- 严禁篡改原始 `data/` 目录下的文件。
- 生成的图表必须包含 `_output` 后缀。
```
</div>

<!--
给大家展示一下怎么把 AI 当"实习生"管。
Skill 机制解决了复杂编排的确定性问题。
有一个最新的开源项目，只有一段提示词，严格约束=可复现的开发流程=固定的产物（甚至是一个app）
-->

---
layout: center
text-center: true
---

# <lucide-trending-up class="inline-block mr-2 mb-1 opacity-70"/>技术趋势：协议层 vs 协议级自治

<div class="max-w-3xl mx-auto mt-12 text-left bg-slate-900/20 p-8 rounded-xl border border-slate-700 relative">
  <div class="absolute -top-4 -right-4"><lucide-eye class="text-4xl text-slate-600 opacity-50" /></div>
  
  <h3 class="text-purple-400 mb-4 font-bold text-sm">如何看待大热的 MCP (Model Context Protocol) 接入标准？</h3>
  <p class="text-sm opacity-80 border-l-2 border-purple-500/50 pl-4 mb-8 leading-relaxed">
    Anthropic 推出的统一工具接口标准，目前正在被各类 IDE 和平台大范围集成。它的目的是解决 AI 与本地资源的授信与暴露问题。
  </p>

  <h3 class="text-green-400 mb-4 font-bold text-sm mt-8">基于终端范式的长期效能：</h3>
  <ul class="text-sm opacity-80 mt-2 space-y-3 relative">
    <li class="flex items-start gap-2"><lucide-circle-dashed class="w-4 h-4 shrink-0 mt-1 text-slate-500"/> <div>一旦模型推理能力跨过某个阈值（例如 DeepSeek R1），它可以原生编写 Shell 脚本直接对接底层 API，免去 MCP 的适配层胶水代码。</div></li>
    <li class="flex items-start gap-2"><lucide-circle-dashed class="w-4 h-4 shrink-0 mt-1 text-slate-500"/> <div>CLI 的标准输入输出 (stdin/stdout) 在过去的极简设计中已经证明了其最高的文本吞吐效率。</div></li>
    <li class="flex items-start gap-2"><lucide-circle-dashed class="w-4 h-4 shrink-0 mt-1 text-slate-500"/> <div><b>工程预判：</b> 繁杂的 API 授权注册将被 AI 自主终端脚本接管，赋予 AI 原生 Shell 权力的方案将成为高效基座。</div></li>
  </ul>
</div>

<!--
这个是一个带有前瞻性和专业性的观点。
-->

---
layout: default
---

# <lucide-server-crash class="inline-block mr-2 mb-1 opacity-70"/>物理瓶颈：上下文窗口过载怎么办？

任何无边界的自动化摄入最终都会撞上 "Context limits" 这面叹息之墙。

<h3 class="mt-8 mb-4 text-sm font-bold opacity-80 pl-2">目前业界的三种长效工程方案对比：</h3>

<div class="grid grid-cols-3 gap-6">
  <div class="bg-slate-800/20 p-5 rounded-lg border border-slate-700">
    <div class="flex items-center gap-2 mb-3">
      <lucide-minimize-2 class="w-5 h-5 text-yellow-500 opacity-80"/> 
      <h3 class="text-sm font-bold text-slate-200">自动摘要压缩</h3>
    </div>
    <div class="text-xs text-slate-400 mb-3 bg-slate-900/50 inline-block px-2 py-1 rounded">Claude Code</div>
    <p class="text-xs opacity-70 leading-relaxed">让 AI 自我提炼上半场上下文，生成摘要存入历史语料。</p>
    <div class="mt-4 text-[10px] text-red-400">缺点：有损压缩，长链路下细节丢失严重。</div>
  </div>

  <div class="bg-blue-900/10 p-5 rounded-lg border border-blue-500/30 relative">
    <div class="flex items-center gap-2 mb-3">
      <lucide-hard-drive class="w-5 h-5 text-blue-400 opacity-80"/> 
      <h3 class="text-sm font-bold text-blue-200">Markdown 长记忆</h3>
    </div>
    <div class="text-xs text-blue-300 mb-3 bg-blue-900/30 inline-block px-2 py-1 rounded border border-blue-500/20">OpenClaw 核心</div>
    <p class="text-xs opacity-70 leading-relaxed">将核心推演、架构与上下文格式化落盘为 .md，无缝衔接。</p>
    <div class="mt-4 text-[10px] text-green-400">目前稳定科研自动化任务的最优解。</div>
  </div>

  <div class="bg-slate-800/20 p-5 rounded-lg border border-slate-700">
    <div class="flex items-center gap-2 mb-3">
      <lucide-database class="w-5 h-5 text-green-500 opacity-80"/> 
      <h3 class="text-sm font-bold text-slate-200">向量化 RAG 检索</h3>
    </div>
    <div class="text-xs text-slate-400 mb-3 bg-slate-900/50 inline-block px-2 py-1 rounded">Cursor Codebase</div>
    <p class="text-xs opacity-70 leading-relaxed">切片源码库与文献集生成 Embedding，利用余弦相似度检索。</p>
    <div class="mt-4 text-[10px] text-red-400">瓶颈：弱相关长依赖（Recall）准确率受限。</div>
  </div>
</div>

<!--
引出上下文瓶颈，也是为了给后面"任务编排极易崩溃"做科学严谨的铺垫。
-->

---
layout: center
---

# <lucide-shield-alert class="inline-block mr-2 mb-1 opacity-70"/>CLI 范式的操作边界

纯终端代理具有极高的算本效率，但同时也受困于物理隔离。

<div class="flex justify-center mt-6">
  <img src="/images/agent_capabilities_circles.png" alt="Agent Capabilities Boundaries" class="w-[360px] h-auto object-cover rounded-full shadow-2xl border border-slate-700/50" />
</div>

<!--
非常有冲击力的画面，用能力同心圆。
指出 CLI 的局限性：无法操作网页上点按钮，由于看不到屏幕也不能做视觉校验等。
铺垫第五章的大跃迁。
-->
