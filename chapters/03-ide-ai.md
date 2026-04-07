---
layout: center
class: text-center
---

# 第三章：IDE 集成 AI
## 协作编程，从"开环"到"闭环"

<div class="mt-8 opacity-50">
  <lucide-terminal-square class="text-6xl mx-auto" />
</div>

---
layout: default
---

# 🤖 让 AI 住进你的编辑器

如果说 Web AI 是"网络外包团队"，那 IDE AI 就是"结对编程的同桌"。

<div class="grid grid-cols-2 gap-8 mt-10">

  <div class="relative overflow-hidden rounded-xl border border-slate-700 bg-slate-800/20 p-6">
    <div class="flex items-center space-x-3 mb-4">
      <div class="w-10 h-10 bg-slate-800 rounded flex items-center justify-center text-slate-300"><lucide-code /></div>
      <h3 class="text-xl m-0 p-0 text-slate-200 font-bold">Cursor</h3>
    </div>
    <ul class="space-y-3 opacity-80 text-sm mt-4">
      <li><b>核心功能：</b> 行内生成与全库检索问答。</li>
      <li><b>迁移成本低：</b> 基于 VS Code 分支，无缝继承插件生态。</li>
      <li><b>定位：</b> 目前最为成熟的个人日常编码工具。</li>
    </ul>
  </div>

  <div class="relative overflow-hidden rounded-xl border border-slate-600 bg-slate-800/40 p-6 shadow-xl">
    <div class="absolute top-0 right-0 bg-slate-700 text-xs px-3 py-1 rounded-bl-lg text-slate-200">现场演示</div>
    <div class="flex items-center space-x-3 mb-4">
      <div class="w-10 h-10 bg-slate-800 rounded flex items-center justify-center text-blue-300"><lucide-orbit /></div>
      <h3 class="text-xl m-0 p-0 text-blue-300 font-bold">Antigravity</h3>
    </div>
    <ul class="space-y-3 opacity-80 text-sm mt-4">
      <li><b>技术背景：</b> Google 内部前沿架构。</li>
      <li><b>核心突破：</b> 支持工程级别的大规模重构。</li>
      <li><b>工作流：</b> 独有的 Planning Mode（人机异步确认机制）。</li>
      <li><b>自治能力：</b> 内置 Headless 浏览器进行效果自测。</li>
    </ul>
  </div>

</div>

<!--
给大家铺垫一下什么是 IDE AI。
重点带出 Antigravity，因为我将用它做接下来的 Live Demo。
（另外简单提及老牌工具 GitHub Copilot 说它注重单行补全即可）
-->

---
layout: center
---

# <lucide-play-circle class="inline-block mr-2 mb-1 opacity-70"/>现场实战：从 0 搭建数据可视化项目

<div class="text-left max-w-xl mx-auto bg-slate-800/30 p-8 rounded border border-slate-700 mt-8">
  <div class="text-slate-300 font-bold mb-4 flex items-center gap-2"><lucide-list-check class="w-5 h-5"/> 演示节点：</div>
  <ol class="space-y-4 opacity-80 text-sm">
    <li>1. 提供包含脏数据的科研 CSV 样本。</li>
    <li>2. 向 Antigravity 输入自然语言指令："解析数据并生成可视化网页"。</li>
    <li>3. 观察 AI 进入 <b>Planning Mode（计划模式）</b>，输出系统架构与修复方案。</li>
    <li>4. 我们评审计划并授权审批 → 观察 AI 执行多文件生成。</li>
    <li><span class="text-blue-300 font-mono tracking-wide">关键观察点：</span> 在执行过程中发生报错，观察 AI 如何读取控制台输出并自动修改修复。</li>
  </ol>
</div>

<p class="mt-8 text-sm opacity-50 italic text-center font-mono">
  Switching to local Antigravity environment...
</p>

<!--
【现场演示环节】
1. 打开 Antigravity。
2. 演示 Planning Mode 的流程，强调"人机审核"的重要性。
3. 演示过程中可能会出现 AI 修改代码。
4. 演示它自己 debug 的一轮闭环。
-->

---
layout: default
---

# <lucide-git-branch class="inline-block mr-2 mb-1 opacity-70"/>核心理论：控制论与反馈回路

> IDE AI 的本质能力并非大模型的单点突破，而是架构层级的进化——引入了"反馈"。

<div class="my-6 flex justify-center w-full overflow-hidden">
  <img src="/images/ide_feedback_loop_horizontal.png" alt="Feedback Loop" class="h-[260px] scale-140 object-cover rounded-lg shadow-xl border border-slate-700/50 opacity-90" />
</div>

<div class="grid grid-cols-2 gap-8 px-8">
  <div>
    <h3 class="text-slate-300 font-bold text-sm border-b border-slate-700 pb-2 mb-3">开环控制（常规 Web）</h3>
    <p class="text-xs opacity-70 leading-relaxed">输出质量高度依赖模型的单次推理准确度（Zero-Shot）。一旦生成结束链条便断裂，必须依赖人工接力排错。</p>
  </div>
  <div>
    <h3 class="text-blue-300 font-bold text-sm border-b border-slate-700 pb-2 mb-3">闭环系统（Feedback Loop）</h3>
    <p class="text-xs opacity-70 leading-relaxed">IDE 将终端报错、编译警告化为自动回流信号。<b>反馈回路的丰富度与速度，决定了智能协作能力的上限。</b></p>
  </div>
</div>

<!--
控制论。
这个图很直观。把 IDE AI 的本质提炼出来了：这不仅是一个模型性能的提升，这是系统架构的进化，引入了"反馈"，其实这不是第一次引入，web 多轮对话本质上也是人类直接给到模型反馈。
区别是，现在模型可以直接接收 ide 的反馈，处理好再给人类汇报，人类的反馈次数减少了。

之前是 AI to 人类，人类 to AI。
现在是 IDE 产物  -   AI  -  人类三方。
-->
