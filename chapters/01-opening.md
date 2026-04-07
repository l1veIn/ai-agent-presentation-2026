---
layout: intro
---

# 我与 AI 工具的日常

> "AI 已经不是我的助手，而是我的数字同事。"

- **日常写代码**：Antigravity & Cursor
- **批量任务处理**：Claude Code & Gemini CLI
- **跨应用复杂执行**：OpenClaw & WorkBuddy
- **文献与创意**：NotebookLM & DeepSeek R1

<div class="mt-8 border-l-4 border-slate-500 pl-4 opacity-75">
  <p><lucide-terminal class="inline-block mr-2 text-slate-400"/><b>今天演示环境：</b> MacOS 本地执行，真实还原数字工作流。</p>
</div>

<!--
演讲者：
简单自我介绍，并且切到 Mac 桌面快速给大家看一眼你的环境配置（例如你的终端、Antigravity 图标等）。
明确告诉大家今天有很多现场实地操作演示。
-->

---
layout: center
---

# <lucide-map class="inline-block mr-2 mb-1 opacity-70"/>今天的探索路线图

一条从"开环"走向"系统闭环"的能力跃迁之路

<div class="flex items-center justify-center mt-6 gap-4">
  <div class="text-center w-52 bg-slate-800/20 p-4 rounded-lg border border-slate-700">
    <lucide-message-square class="text-3xl mb-3 mx-auto text-blue-400 opacity-80" />
    <div class="font-bold text-lg text-slate-200">第一阶：Web 对话</div>
    <div class="text-xs mt-2 opacity-60">"我说，它答"</div>
    <div class="text-[10px] mt-3 text-slate-500">ChatGPT / DeepSeek</div>
  </div>
  <div class="text-2xl text-slate-600 shrink-0">→</div>
  <div class="text-center w-52 bg-slate-800/20 p-4 rounded-lg border border-slate-700">
    <lucide-terminal-square class="text-3xl mb-3 mx-auto text-cyan-400 opacity-80" />
    <div class="font-bold text-lg text-slate-200">第二阶：IDE & CLI</div>
    <div class="text-xs mt-2 opacity-60">"我说，它做"</div>
    <div class="text-[10px] mt-3 text-slate-500">Antigravity / Claude Code</div>
  </div>
  <div class="text-2xl text-slate-600 shrink-0">→</div>
  <div class="text-center w-52 bg-slate-800/20 p-4 rounded-lg border border-slate-700">
    <lucide-cpu class="text-3xl mb-3 mx-auto text-purple-400 opacity-80" />
    <div class="font-bold text-lg text-slate-200 pb-1">第三阶：Computer Use</div>
    <div class="text-xs mt-2 opacity-60">"接管操作系统"</div>
    <div class="text-[10px] mt-3 text-slate-500">OpenClaw / OS控制</div>
  </div>
</div>

<div class="text-center mt-12 text-sm opacity-50 uppercase tracking-widest font-mono text-xs">
  信息论 — 控制论 — 系统论
</div>

<!--
这一页是全局导航，让大家心中有数。
引导听众注意"三级跃迁"的概念，这是整场 PPT 的叙事脊梁。预告接下来的理论彩蛋。
-->

---
layout: center
---

# <lucide-users class="inline-block mr-2 mb-1 opacity-70"/>团队现状自测

### 凭第一直觉，你/你的组最近最常用哪类 AI 工具？

<div class="grid grid-cols-2 gap-4 mt-8 max-w-3xl mx-auto">
  <div class="bg-gray-800/30 p-4 rounded text-center border border-slate-700">
    <span class="text-base">A. 官方 Web 界面 (ChatGPT等)</span>
  </div>
  <div class="bg-gray-800/30 p-4 rounded text-center border border-slate-700">
    <span class="text-base">B. 代码编辑器辅助 (Cursor等)</span>
  </div>
  <div class="bg-gray-800/30 p-4 rounded text-center border border-slate-700">
    <span class="text-base">C. 终端独立 Agent (Claude Code等)</span>
  </div>
  <div class="bg-gray-800/30 p-4 rounded text-center border border-slate-700 text-slate-500">
    <span class="text-base">D. 没深度用过 / 仅停留在搜索</span>
  </div>
</div>

<p class="text-center mt-12 text-sm text-slate-400">
  了解不同的认知起点，我们今天重点解决从 A 到 B、从 B 到 C 的痛点。
</p>

<!--
现场互动时间。可以举手投票，或者让他们心中有数。
引语：如果只有选 A 的经历，那你今天可能要经历巨大的认知升级了。
-->

---
layout: two-cols
---

# <lucide-wifi class="inline-block mr-2 mb-1 opacity-70"/>前置：稳定的网络环境
### AI 工具链的基石

模型 API 的稳定性不仅决定了单个查询的成功率，更决定了长链路自动化的可能。
校园或企业网环境下的抖动，会成倍放大自动化任务的错误率。

<div class="mt-8 bg-slate-900/40 p-5 rounded-lg border border-slate-700">
  <h3 class="text-cyan-400 mb-3 text-sm font-bold"><lucide-server class="inline-block mr-1"/> 建议架构：独立 4G/5G 软路由网关</h3>
  <ul class="space-y-3 opacity-80 text-sm mt-4">
    <li class="flex items-start gap-2"><lucide-check-circle class="text-green-500 w-4 h-4 mt-1"/> <div><b>物理隔离稳定性：</b> 远高于热点桥接，保障极长上下文（Long-Context）传输不断流。</div></li>
    <li class="flex items-start gap-2"><lucide-check-circle class="text-green-500 w-4 h-4 mt-1"/> <div><b>透明代理机制：</b> 终端、IDE 等非浏览器环境"无感"直连，杜绝繁琐的环境变量设置。</div></li>
    <li class="flex items-start gap-2"><lucide-check-circle class="text-green-500 w-4 h-4 mt-1"/> <div><b>智能分流策略：</b> API 请求与其他服务分流处理，不增加额外网络延迟。</div></li>
  </ul>
</div>

::right::

<div class="h-full flex flex-col justify-center items-center p-8">
  <div class="w-full bg-slate-800/50 p-6 rounded-lg text-center font-mono text-sm leading-relaxed border border-slate-700">
    <div class="text-gray-400 mb-2">My Mac</div>
    <div class="text-2xl text-blue-400">↓ WiFi</div>
    <div class="bg-blue-900/40 border border-blue-500/50 p-3 rounded my-2 font-bold text-white">4G 软路由网关</div>
    <div class="text-2xl text-purple-400">↓ 4G Network</div>
    <div class="text-gray-400 mt-2">Internet / Claude / GPT API</div>
  </div>
  
  <p class="mt-6 text-sm text-slate-400 italic">
    * 提示：对于国内同学，这是全自动工作流能稳定运行的基石。（或者直接使用全国产方案！）
  </p>
</div>

<!--
这是硬核实操经验。
（现场你可以指一下你带的 4G 软路由"就是这个小盒子"）。
解释为什么不用手机热点（会发烫、会降频断流、终端代理配置麻烦）。
强调一下透明代理的好处，这是后面玩 Agent 的基础设施。
-->
