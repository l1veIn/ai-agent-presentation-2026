---
layout: center
class: text-center
---

# 第二章：Web 对话式 AI
## 最低门槛的切入点

（这可能是我们在座 90% 同学每天在用的形态）

<div class="mt-8 opacity-50">
  <lucide-messages-square class="text-6xl mx-auto" />
</div>

---
layout: default
---

# <lucide-globe class="inline-block mr-2 mb-1 opacity-70"/>对话式大模型概览：没有"最好"，只看"最合适"

<div class="grid grid-cols-3 gap-6 mt-6">
  <div class="bg-slate-800/20 p-5 rounded-xl border border-slate-700">
    <h3 class="text-lg mb-2 text-blue-300 font-bold">ChatGPT (OpenAI)</h3>
    <ul class="text-xs opacity-70 space-y-2 mt-3">
      <li><b>推荐:</b> ChatGPT Codex 5.4</li>
      <li><b>擅长:</b> 复杂逻辑链推演、代码结构重构</li>
      <li><b>特色:</b> 代码与文本混合生态的绝对霸主</li>
    </ul>
  </div>
  <div class="bg-slate-800/20 p-5 rounded-xl border border-slate-700">
    <h3 class="text-lg mb-2 text-orange-300 font-bold">Claude (Anthropic)</h3>
    <ul class="text-xs opacity-70 space-y-2 mt-3">
      <li><b>推荐:</b> Claude Opus 4.6 / Sonnet 3.7</li>
      <li><b>擅长:</b> 极长上下文开发、细腻的语言风格把控</li>
      <li><b>特色:</b> Artifacts 可视化与前沿的控制阈值</li>
    </ul>
  </div>
  <div class="bg-slate-800/20 p-5 rounded-xl border border-slate-700">
    <h3 class="text-lg mb-2 text-blue-200 font-bold">Gemini (Google)</h3>
    <ul class="text-xs opacity-70 space-y-2 mt-3">
      <li><b>推荐:</b> Gemini 3.1 Pro</li>
      <li><b>擅长:</b> 原生多模态解析（视频/视觉日志排查）</li>
      <li><b>特色:</b> 海量 Token 吸收和全家桶整合</li>
    </ul>
  </div>
</div>

<h2 class="mt-8 mb-4 text-lg font-bold text-slate-300"><lucide-flag class="inline-block mr-2 w-5 h-5"/>国产矩阵 — 科研生产力的重要平替</h2>

<div class="grid grid-cols-4 gap-3 text-xs mt-4">
  <div class="bg-slate-800/20 p-4 rounded-lg border border-slate-700">
    <div class="font-bold text-slate-200 text-sm">DeepSeek</div>
    <div class="opacity-60 mt-2 leading-relaxed"><b>V3/R1 架构</b>｜极高的推理性价比，私有化部署和微调的第一选择。</div>
  </div>
  <div class="bg-slate-800/20 p-4 rounded-lg border border-slate-700">
    <div class="font-bold text-slate-200 text-sm">豆包 (字节)</div>
    <div class="opacity-60 mt-2 leading-relaxed">高并发极验，接口稳定性顶尖，适合大批量文本清洗预处理。</div>
  </div>
  <div class="bg-slate-800/20 p-4 rounded-lg border border-slate-700">
    <div class="font-bold text-slate-200 text-sm">通义千问 (阿里)</div>
    <div class="opacity-60 mt-2 leading-relaxed">Qwen 生态丰富，端侧小模型与开源全家桶适配性极佳。</div>
  </div>
  <div class="bg-slate-800/20 p-4 rounded-lg border border-slate-700">
    <div class="font-bold text-slate-200 text-sm">智谱 GLM</div>
    <div class="opacity-60 mt-2 leading-relaxed">针对中文学术语料与科研论文检索做了原生级的数据优化。</div>
  </div>
</div>

<!--
给大家快速过一下目前有哪些趁手的工具。
特别是对于 AI 学院的同学。
-->

---
layout: two-cols
---

# <lucide-terminal class="inline-block mr-2 mb-1 opacity-70"/>实战对比：文献调研的提示词工程

**场景：** 调研多模态大模型幻觉问题的最新研究。

<div class="mt-8 pr-4">
<h3 class="text-slate-400 font-bold mb-3 text-sm flex items-center gap-2"><lucide-x-circle class="text-slate-500 w-4 h-4"/> 模糊的开环请求</h3>
<div class="bg-slate-900 p-4 rounded text-xs font-mono opacity-60 border-l border-slate-600">
"帮我找一下多模态大模型幻觉的相关论文"
</div>
<div class="mt-4 text-xs text-slate-500 italic">
结果往往是百科式的泛泛之谈，无具体信源。
</div>
</div>

::right::

<div class="h-full flex flex-col justify-center pl-8 pt-10">
<h3 class="text-blue-400 font-bold mb-3 text-sm flex items-center gap-2"><lucide-check-circle class="w-4 h-4"/> 高潜能的参数化约束请求</h3>
<div class="bg-slate-900 p-4 rounded text-[11px] font-mono border-l-2 border-blue-500 text-blue-100 leading-relaxed shadow-lg">
"你是一位计算视觉资深研究员。我正在调研多模态大模型 (如 LLaVA) 中的幻觉问题。<br><br>任务：<br>1. 梳理过去 12 个月的 5 篇顶会改进论文。<br>2. 按照'评估方法 -> 现象成因 -> 缓解策略'表述。<br>3. 格式：严格学术风格，嵌入 [第一作者, 年份] 引用标识。"
</div>

<p class="mt-8 text-sm text-slate-300 font-mono tracking-wide border-l-2 border-slate-500 pl-4 py-1">
信息密度的差异决定了对话模型的行为边界。
</p>
</div>

<!--
引出理论。

这个例子非常有效，可以在 web、IDE、OpenClaw、NotebookLM 都用同样的提示词执行这个任务。可以对比不同工具的抓手和落点。能让观众理解编排行为的产生。
-->

---
layout: default
---

# <lucide-share-2 class="inline-block mr-2 mb-1 opacity-70"/>香农信道模型在 Prompt 中的映射

> 从通信理论视角理解：不要把对话模型当成具象的实体，而将其视为一条信道。

<div class="flex items-center justify-center my-8">
<div class="font-mono text-sm tracking-tight text-center bg-slate-900/40 p-8 rounded-xl border border-slate-700 w-full max-w-4xl relative overflow-hidden">
<div class="flex justify-between items-center relative z-10">
  <div class="p-4 bg-slate-800/50 rounded-lg border border-slate-700">
    <div class="text-base font-bold text-slate-200 mb-1">物理端 (信源)</div>
    <div class="opacity-50 text-xs">你的科研或开发意图</div>
  </div>
  <div class="flex-1 px-4 relative mt-2">
    <div class="h-[2px] bg-slate-600 relative">
      <div class="absolute -top-6 left-1/4 bg-slate-800 border border-slate-600 px-2 py-1 rounded text-[10px] text-slate-300">Prompt = 编码</div>
      <div class="absolute -top-6 right-1/4 bg-slate-800 border border-slate-600 px-2 py-1 rounded text-[10px] text-slate-300">Response = 解码</div>
      <div class="absolute top-3 left-1/2 -translate-x-1/2 flex items-center gap-1 text-[10px] text-slate-500 bg-slate-900 px-2 py-0.5 rounded border border-slate-700">
        <lucide-alert-circle class="w-3 h-3" /> 漂移/信息压缩
      </div>
    </div>
  </div>
  <div class="p-4 bg-slate-800/50 rounded-lg border border-slate-700">
    <div class="text-base font-bold text-slate-200 mb-1">推理端 (信道)</div>
    <div class="opacity-50 text-xs">带宽 = Context Window</div>
  </div>
</div>
</div>
</div>

### Prompt 工程的核心：极大化信噪比 (SNR)
- **优质 Prompt (高 SNR)** = 显式化隐藏条件，抑制幻觉产生。
- **长度与损耗机制**：并不是丢的参数越多越好，冗余信息过载同样会导致模型在中段检索能力的自然丢失 (Lost in the Middle现象)。

<!--
通信模型。
-->

---
layout: center
class: text-center
---

# Web 范式的物理边界在哪里？

<div class="relative w-[600px] mx-auto mt-12 bg-slate-900/40 p-8 rounded-xl border border-slate-700">
  <div class="flex justify-between items-center text-sm font-mono mb-6">
    <div class="text-slate-300 border px-3 py-2 rounded border-slate-600 bg-slate-800/50">输入 (Prompt)</div>
    <div class="text-xl text-slate-500">─→</div>
    <div class="text-slate-200 font-bold text-lg"><lucide-cpu class="inline-block mr-1 opacity-50"/> 推理侧</div>
    <div class="text-xl text-slate-500">─→</div>
    <div class="text-slate-300 border px-3 py-2 rounded border-slate-600 bg-slate-800/50">输出片段</div>
  </div>
  
  <div class="text-slate-400 text-xs tracking-wider uppercase border-t border-slate-700 pt-4 flex justify-center items-center gap-2">
    <lucide-git-commit class="w-4 h-4"/> 单向开环系统 (Open Loop)
  </div>
</div>

<ul class="text-left max-w-xl mx-auto mt-12 space-y-3 opacity-70 text-sm">
  <li class="flex items-start gap-2"><lucide-minus class="text-slate-500 w-4 h-4 mt-0.5 shrink-0"/> <b>人工闭环依赖：</b> 复制生成代码 → 手动运行 → 手动排查 → 手动回传错误给模型。</li>
  <li class="flex items-start gap-2"><lucide-minus class="text-slate-500 w-4 h-4 mt-0.5 shrink-0"/> <b>短时记忆灾难：</b> 会话结束即断联，缺乏整个项目的长效物理状态追踪。</li>
  <li class="flex items-start gap-2"><lucide-minus class="text-slate-500 w-4 h-4 mt-0.5 shrink-0"/> <b>仅停留在表述：</b> 它只能给出规划建议，而没有"执行键"。</li>
</ul>

<p class="mt-12 text-cyan-400 font-medium tracking-wide">
  "如果让 AI 拥有一个编辑器，自己看着报错改代码呢？"
</p>

<!--
承上启下的关键页。
点出 Web 对话的痛点：你要一直做搬运工。
因为它是"开环"的。
引出下一章 IDE AI。
-->

---
layout: center
---

<div class="w-[50vw] h-[50vh] -mt-4 -mx-4" style="margin: -16px;">
  <iframe 
    src="./ranking.html"
    width="100%" 
    height="100%" 
    frameborder="0"
  ></iframe>
</div>

<!--
【现场互动环节】
现在你已经了解了各种模型的特点，凭直觉给它们排位吧！
全屏沉浸式天梯，无标题无边框干扰。
操作方式：
1. 进入此页后，直接拖动卡片到天梯层级（夯/顶级/人上人/NPC/拉完了）
2. 记录投票分布
3. 留下悬念："听完后面几章，你的排序会变吗？"

重点观察：
- 国产模型 vs 海外模型的认知差距
- 有没有同学把 DeepSeek/Kimi 放到最高层级
-->
