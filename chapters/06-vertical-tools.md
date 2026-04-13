---
layout: center
class: text-center
---

# 第六章：垂直工具与工作流拼图
## 从单点突破走向全域体系

<div class="mt-12 text-5xl opacity-40 text-cyan-400">
  <lucide-blocks class="mx-auto" />
</div>

---
layout: default
---

# <lucide-hammer class="inline-block mr-2 mb-1 opacity-70"/>垂直领域工具群落：不盲目依赖单一基座

<div class="grid grid-cols-2 gap-6 mt-8">
  <div class="bg-slate-800/20 p-5 rounded-lg border border-slate-700 flex gap-4 min-h-[9rem]">
    <div class="text-slate-500 pt-1"><lucide-library class="w-6 h-6" /></div>
    <div>
      <h3 class="font-bold text-lg text-slate-200">NotebookLM (Google)</h3>
      <div class="text-xs opacity-60 mb-3 border-l-2 border-slate-500 pl-2">文献本体推理</div>
      <p class="text-xs opacity-70 leading-relaxed">导入海量 PDF 源数据，支持生成跨引用的超长音频播客。因推理被强约束在源文档库中，幻觉概率极低。</p>
    </div>
  </div>

  <div class="bg-slate-800/20 p-5 rounded-lg border border-slate-700 flex gap-4 min-h-[9rem]">
    <div class="text-slate-500 pt-1"><lucide-pen-tool class="w-6 h-6" /></div>
    <div>
      <h3 class="font-bold text-lg text-slate-200">Lovart</h3>
      <div class="text-xs opacity-60 mb-3 border-l-2 border-slate-500 pl-2">专业排版与海报生成</div>
      <p class="text-xs opacity-70 leading-relaxed">相较于主流纯绘图工具，具有明确的结构学对齐设计逻辑，适合科研信息流排版分发。</p>
    </div>
  </div>

  <div class="bg-slate-800/20 p-5 rounded-lg border border-slate-700 flex gap-4 min-h-[9rem] relative overflow-hidden">
    <div class="text-slate-500 pt-1"><lucide-search class="w-6 h-6" /></div>
    <div>
      <h3 class="font-bold text-lg text-slate-200">秘塔 AI 搜索 / Perplexity</h3>
      <div class="text-xs opacity-60 mb-3 border-l-2 border-slate-500 pl-2">带脚标强约束引擎</div>
      <p class="text-xs opacity-70 leading-relaxed">彻底颠覆宽泛搜索习惯。极速抓取外部世界实时知识并强生成反幻觉引文标识。</p>
    </div>
  </div>

  <div class="bg-slate-800/20 p-5 rounded-lg border border-slate-700 flex gap-4 min-h-[9rem] relative">
    <div class="absolute -left-1 text-[9px] bg-slate-700 px-1 py-0.5 rounded-r text-slate-300 shadow top-3 whitespace-nowrap opacity-80">老牌复读</div>
    <div class="text-slate-500 pt-1 pl-3"><lucide-file-edit class="w-6 h-6" /></div>
    <div>
      <h3 class="font-bold text-lg text-slate-200">Grammarly</h3>
      <div class="text-xs opacity-60 mb-3 border-l-2 border-slate-500 pl-2">最终收口的润色门卫</div>
      <p class="text-xs opacity-70 leading-relaxed">大模型可以提供写作思路，但论文完稿（Camera Ready）前的标点符号校正和句法合规确认，离不开专职的细粒度打磨网络。</p>
    </div>
  </div>
</div>

<!--
NotebookLM 重点演示
-->

---
layout: center
---

# <lucide-git-merge class="inline-block mr-2 mb-1 opacity-70"/>集成思路：组合你的管线生态流

<div class="bg-slate-900/40 rounded-xl p-6 border border-slate-700 mt-8 relative">
  <div class="mb-4 opacity-70 text-sm border-l-2 border-slate-500 pl-4 font-mono tracking-wide">"架构设计是做减法，选用匹配当前阶段最佳组合。"</div>
  <div class="space-y-6 w-full mt-8">
    <!-- Workflow A -->
    <div class="group">
      <div class="text-xs font-bold text-slate-400 tracking-wider mb-2">流派 A: 数据挖掘与实验派</div>
      <div class="flex items-center gap-2 font-mono text-xs overflow-x-auto pb-1 scrollbar-hide">
        <div class="bg-slate-800 text-slate-300 border border-slate-600 px-3 py-1.5 rounded shrink-0">1. NotebookLM (源语料整合)</div>
        <div class="text-slate-600 shrink-0">→</div>
        <div class="bg-slate-800 text-slate-300 border border-slate-600 px-3 py-1.5 rounded shrink-0">2. Code Interpreter (脚本算力)</div>
        <div class="text-slate-600 shrink-0">→</div>
        <div class="bg-slate-800 text-slate-300 border border-slate-600 px-3 py-1.5 rounded shrink-0">3. Opus 4.6 (逻辑降噪输出)</div>
      </div>
    </div>
    <!-- Workflow B -->
    <div class="group">
      <div class="text-xs font-bold text-slate-400 tracking-wider mb-2">流派 B: 前沿架构开发派</div>
      <div class="flex items-center gap-2 font-mono text-xs overflow-x-auto pb-1 scrollbar-hide">
        <div class="bg-slate-800 text-slate-300 border border-slate-600 px-3 py-1.5 rounded shrink-0">1. Claude Code (CLI批量脚手架)</div>
        <div class="text-slate-600 shrink-0">→</div>
        <div class="bg-slate-800 text-slate-300 border border-slate-600 px-3 py-1.5 rounded shrink-0">2. Antigravity IDE (领域架构大调)</div>
        <div class="text-slate-600 shrink-0">→</div>
        <div class="bg-slate-800 text-slate-300 border border-slate-600 px-3 py-1.5 rounded shrink-0">3. OpenClaw (虚拟机隔离验证)</div>
      </div>
    </div>
    <!-- Workflow C -->
    <div class="group">
      <div class="text-xs font-bold text-slate-400 tracking-wider mb-2 flex items-center gap-2"><lucide-shield-check class="w-4 h-4"/> 泛用兜底：断网/校网脱壳全直连链条</div>
      <div class="flex items-center gap-2 font-mono text-xs overflow-x-auto pb-1 scrollbar-hide">
        <div class="bg-slate-800 text-slate-300 border border-slate-600 px-3 py-1.5 rounded shrink-0">1. 秘塔长效聚合搜</div>
        <div class="text-slate-600 shrink-0">→</div>
        <div class="bg-slate-800 text-slate-300 border border-slate-600 px-3 py-1.5 rounded shrink-0">2. DeepSeek R1 满血版算力突破</div>
        <div class="text-slate-600 shrink-0">→</div>
        <div class="bg-slate-800 text-slate-300 border border-slate-600 px-3 py-1.5 rounded shrink-0">3. 豆包平台工作台编发</div>
      </div>
    </div>
  </div>
</div>

<!--
这是 AI 工作流，还可以提一嘴 N8N\Dify 这种，也是“AI 工作流”，更准确的说是“包含 AI”的自动工作流，强调自动执行，强调包含 AI 节点。
-->
