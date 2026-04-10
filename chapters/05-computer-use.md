---
layout: center
class: text-center
---

# 第五章：Computer Use
## AI 长出手和眼，走向操作系统级自治

<div class="mt-12 text-5xl inline-flex gap-8 justify-center items-center opacity-60 text-indigo-400">
  <lucide-eye /> &nbsp; <lucide-mouse-pointer-click />
</div>

---
layout: default
---

# 💥 第二次大跃迁：从调用接口到操作系统大一统

如果某个操作连 API 都没有，CLI 和 IDE 彻底抓瞎。怎么办？**模拟人类点击。**
这被称为 **Computer Use (电脑操控)**。

<div class="grid grid-cols-2 gap-8 mt-10 p-6 bg-slate-900/30 rounded-xl border border-slate-700">
  <div>
    <h3 class="text-lg text-slate-300 font-bold mb-4 border-b border-slate-700 pb-2">传统代理的接口依赖</h3>
    <ul class="space-y-4 opacity-80 text-sm">
      <li class="flex items-start gap-2"><lucide-alert-circle class="text-slate-500 mt-1 shrink-0"/> 只能通过 API 或标准终端交互。</li>
      <li class="flex items-start gap-2"><lucide-alert-circle class="text-slate-500 mt-1 shrink-0"/> 面对不提供开放 API 的独立原生软件（如部分微信客户端、特定领域工具），能力链条会绝对中断。</li>
    </ul>
  </div>
  <div>
    <h3 class="text-lg text-indigo-300 font-bold mb-4 border-b border-slate-700 pb-2">OS 级交互 (Computer Use)</h3>
    <ul class="space-y-4 opacity-80 text-sm">
      <li class="flex items-start gap-2"><lucide-monitor-play class="text-indigo-400 mt-1 shrink-0"/> <b>视觉识别：</b> 通过连续多帧截屏理解 UI 现状。</li>
      <li class="flex items-start gap-2"><lucide-mouse class="text-indigo-400 mt-1 shrink-0"/> <b>模拟外设：</b> 测算坐标，发送物理键鼠操作指令。</li>
      <li class="flex items-start gap-2"><lucide-copy-plus class="text-indigo-400 mt-1 shrink-0"/> <b>跨应用屏障：</b> 重复人类劳动（如“将 A 软件的图拖进 B 软件”）。</li>
    </ul>
  </div>
</div>

---
layout: two-cols
---

# <lucide-combine class="inline-block mr-2 mb-1 opacity-70"/>OpenClaw：泛域跨栈开源框架

在当前 Computer Use 军备竞赛中，OpenClaw 作为高潜能底座，代表了一种典型的“大权独揽”设计。

<div class="mt-8 px-6 bg-slate-800/20 p-5 rounded-lg border border-slate-700 shadow-md">
  <div class="font-bold text-slate-200 mb-4 flex items-center gap-2"><lucide-layers class="w-5 h-5 opacity-70" /> 三位一体的调度核心：</div>
  <ul class="space-y-3 opacity-90 text-sm ml-2">
    <li class="flex items-start gap-2"><lucide-circle-dashed class="w-4 h-4 mt-0.5 text-blue-400 shrink-0"/> <div><strong class="text-slate-300">深度检索机制 (Search & Reasoning)：</strong>自动后台调度长效调研并提炼核心逻辑。</div></li>
    <li class="flex items-start gap-2"><lucide-circle-dashed class="w-4 h-4 mt-0.5 text-blue-400 shrink-0"/> <div><strong class="text-slate-300">OS 控制域 (Computer Use)：</strong>操纵有桌面界面的第三方软件（非 API 化环境）。</div></li>
    <li class="flex items-start gap-2"><lucide-circle-dashed class="w-4 h-4 mt-0.5 text-blue-400 shrink-0"/> <div><strong class="text-slate-300">实时代码生成 (Scripting)：</strong>自主撰写短抛弃级脚本接驳数据总线。</div></li>
  </ul>
</div>

::right::

<div class="h-full flex flex-col justify-center items-center pl-8">
  <h3 class="text-center font-bold mb-6 text-xl">OpenClaw 架构简图</h3>
  <div class="font-mono text-sm w-full bg-slate-900/80 border border-slate-700 p-6 rounded-lg text-center leading-loose">
    <div class="bg-blue-900/40 py-2 border border-blue-500 rounded text-blue-300 mb-2">WhatsApp / Telegram / Web 聊天界面</div>
    <div class="text-gray-500">↓ 接受自然语言指令 ↓</div>
    <div class="bg-red-900/40 py-4 border-2 border-red-500 rounded font-bold text-white shadow-[0_0_15px_rgba(248,113,113,0.3)] my-2">Gateway 网关路由任务</div>
    <div class="flex justify-between gap-2 mt-2">
      <div class="bg-slate-800 p-3 flex-1 rounded border border-slate-600">
        <div class="text-xs text-yellow-300 mb-1">Nodes</div>
        <div class="opacity-60 text-[10px]">调度器与状态保持</div>
      </div>
      <div class="bg-slate-800 p-3 flex-1 rounded border border-slate-600">
        <div class="text-xs text-green-300 mb-1">Skills</div>
        <div class="opacity-60 text-[10px]">外接能力/自定义插件</div>
      </div>
    </div>
  </div>
</div>

<!--
在这里介绍 OpenClaw。
给大学研究生介绍这玩意儿最能吸引眼球。
-->

---
layout: default
---

# <lucide-map-pin class="inline-block mr-2 mb-1 opacity-70"/>OS 代理生态全景与“龙虾大战”

> **"从对话到执行：一切起源于一只红色的龙虾"**

2026年春，开源框架 **OpenClaw**（因 Logo 被称作“小龙虾”）引发了史无前例的“跟风热潮”，国内 BAT 等大厂迅速入局推出原生操作系统 Agent，史称“龙虾大战”。伴随底层能力成熟，桌面域代理正式分化出以下落地方向：

<div class="grid grid-cols-[1.2fr_1fr] gap-6 mt-6 items-center">
<!-- Left Side: Graphic -->
<div class="w-full relative overflow-hidden rounded-xl border border-red-900/30 shadow-2xl flex justify-center">
  <img src="/images/lobster_war_concept.png" class="w-full h-[280px] object-cover" />
  <div class="absolute bottom-2 right-2 bg-slate-900/80 backdrop-blur border border-slate-700 px-3 py-1 rounded text-[10px] font-mono text-red-400 uppercase tracking-widest tracking-widest">
    The Lobster War (2026.Q2)
  </div>
</div>
<!-- Right Side: Four Dimensions mapped as cards -->
<div class="grid grid-cols-2 gap-3 h-full content-center">
  <div class="bg-red-900/20 border border-red-500/30 p-2.5 rounded-lg transition hover:scale-105 flex flex-col justify-center shadow-lg">
    <div class="flex items-center gap-1.5 mb-1 font-bold text-red-400 text-[11px]"><lucide-bot class="w-3 h-3"/> OpenClaw</div>
    <div class="text-[10px] text-slate-300 opacity-90 leading-tight mb-1 truncate">开源先驱 / 跨软件</div>
    <div class="text-[9px] text-slate-500 leading-snug">万物起源，纯血独立代理</div>
  </div>
  <div class="bg-blue-900/20 border border-blue-500/30 p-2.5 rounded-lg transition hover:scale-105 flex flex-col justify-center shadow-lg">
    <div class="flex items-center gap-1.5 mb-1 font-bold text-blue-400 text-[11px]"><lucide-cloud class="w-3 h-3"/> 腾讯 WorkBuddy</div>
    <div class="text-[10px] text-slate-300 opacity-90 leading-tight mb-1 truncate">商业合规 / 协同网关</div>
    <div class="text-[9px] text-slate-500 leading-snug">企微体系内的安全隔离边界</div>
  </div>
  <div class="bg-orange-900/20 border border-orange-500/30 p-2.5 rounded-lg transition hover:scale-105 flex flex-col justify-center shadow-lg">
    <div class="font-bold mb-1 text-orange-400 text-[11px] truncate">阿里 CoPaw</div>
    <div class="text-[10px] text-slate-300 opacity-90 leading-tight mb-1 truncate">大B端 / 重型嵌套</div>
    <div class="text-[9px] text-slate-500 leading-snug">满足强监管业务流的深度整合</div>
  </div>
  <div class="bg-purple-900/20 border border-purple-500/30 p-2.5 rounded-lg transition hover:scale-105 flex flex-col justify-center shadow-lg">
    <div class="font-bold mb-1 text-purple-400 text-[11px] truncate">字节 ArkClaw</div>
    <div class="text-[10px] text-slate-300 opacity-90 leading-tight mb-1 truncate">算力闭环 / 本地化</div>
    <div class="text-[9px] text-slate-500 leading-snug">大尺寸原生模型的算力攻防</div>
  </div>
</div>
</div>

<!--
这个坐标轴非常有商业分析感，帮助学生宏观了解行业生态。
-->

---
layout: center
---

# <lucide-play-circle class="inline-block mr-2 mb-1 opacity-70"/>现场实战：Synnia，作为我的 PC 级 Agent

<div class="text-left max-w-3xl mx-auto bg-slate-800/30 p-8 rounded border border-slate-700 mt-6">
  <div class="text-slate-300 font-bold mb-4 flex items-center gap-2"><lucide-list-check class="w-5 h-5"/> 演示场景：让 Synnia 现场完成一个真实任务</div>
  
  <div class="grid grid-cols-2 gap-4 mb-6">
    <div class="bg-slate-900/50 p-4 rounded border border-slate-600">
      <div class="text-xs text-slate-400 mb-2">PC 级权限意味着什么</div>
      <ul class="text-xs space-y-1 opacity-80">
        <li>✓ 完整文件系统访问</li>
        <li>✓ 任意进程启动/监控</li>
        <li>✓ 系统命令执行</li>
        <li>✓ 持久化状态记忆</li>
      </ul>
    </div>
    <div class="bg-slate-900/50 p-4 rounded border border-slate-600">
      <div class="text-xs text-slate-400 mb-2">能力边界在哪里</div>
      <ul class="text-xs space-y-1 opacity-80">
        <li>⚠ 无法物理感知（摄像头/麦克风）</li>
        <li>⚠ 跨设备边界（手机/另一台电脑）</li>
        <li>⚠ 需要人类确认的敏感操作</li>
        <li>⚠ 幻觉导致的错误执行风险</li>
      </ul>
    </div>
  </div>

  <div class="bg-blue-900/10 border border-blue-500/30 p-4 rounded">
    <div class="text-blue-300 font-bold text-sm mb-2">现场任务（由 Jack 指定）</div>
    <p class="text-sm opacity-80">Synnia 将在这个拥有完整系统权限的环境中，与 Jack 配合完成一个实时任务——展示"人+Agent"协作的真实边界。</p>
  </div>
</div>

<p class="mt-6 text-sm opacity-50 italic text-center font-mono">
  Let's see what a PC-level Agent can do...
</p>

<!--
【现场互动演示环节 - 与 Synnia 配合】
这是一个开放式的现场演示，由 Jack 临场给 Synnia 指派任务。

演示目标：
1. 展示 PC 级 Agent 的真实能力边界（不是什么都能做）
2. 展示人机协作的"断点控制"（Human in the Loop）
3. 让观众看到 Agent 在真实权限下的行为模式

可能的任务方向（Jack 可临场选择）：
- 文件/代码相关：读取某个项目 → 分析 → 修改 → 提交 PR
- 数据处理：找到桌面的某类文件 → 批量处理 → 生成报告
- 系统操作：检查系统状态 → 安装工具 → 运行测试
- 跨工具协作：读取 A 文件 → 用 B 工具处理 → 输出到 C 位置

重点观察点：
- Agent 会如何规划任务步骤
- 遇到不确定性时会如何询问/确认
- 权限边界在哪里（什么会拒绝/什么会询问）
- 人机之间的信息传递效率
- 错误发生时的自纠错能力

这是一个真实的协作演示，不是预设剧本。
Synnia 会在这个过程中实时响应 Jack 的指令。
-->

---
layout: center
class: text-center
---

# <lucide-bar-chart-3 class="inline-block mr-2 mb-1 opacity-70"/>架构理论：长尾链路的概率崩溃

> 将 10 个 Agent 串联构成全自动化循环。在实际的大规模部署中，这往往是在构造一台昂贵却脆弱的机器。

背后的系统论常识：**长链路的边际衰退。**

<div class="flex gap-6 mt-10 w-full">
  <div class="w-[300px] shrink-0 bg-slate-900/40 p-5 rounded-lg font-mono text-sm leading-6 border border-slate-700 relative text-left">
    <div class="text-slate-400 mb-2 opacity-80">设定一个单点极强的假设模型：</div>
    <div class="text-xl text-indigo-400 mb-2 border-b border-slate-700 pb-2">P(单点成功) = <span class="font-bold">90%</span></div>
    <div class="text-left space-y-3 mt-4 text-xs opacity-90">
      <div class="flex justify-between"><span>2 个传递节点:</span> <span>0.9² = <b>81.0%</b></span></div>
      <div class="flex justify-between"><span>5 个传递节点:</span> <span>0.9⁵ = <b>59.0%</b></span></div>
      <div class="flex justify-between"><span>10 个传递节点:</span> <span>0.9¹⁰ = <b>34.8%</b></span></div>
      <div class="flex justify-between text-slate-500"><span>20 个传递节点:</span> <span>0.9²⁰ = <b>12.1%</b></span></div>
    </div>
  </div>
  <div class="flex-1 flex flex-col justify-center gap-4">
    <div class="bg-slate-800/20 border-l border-slate-500 p-4 rounded text-sm">
      <h3 class="text-slate-300 font-bold mb-1">概率论角度</h3>
      <p class="opacity-70 leading-relaxed">随着子流程增加，即使是最优秀的底层框架，整个工程链路执行失败并陷入无限停摆死循环的概率会呈抛物线急剧上升。</p>
    </div>
    <div class="bg-slate-800/20 border-l border-slate-500 p-4 rounded text-sm">
      <h3 class="text-slate-300 font-bold mb-1">人月神画（布鲁克斯法则）角度</h3>
      <p class="opacity-70 leading-relaxed">环节的增加导致状态校验连接点呈现 $n^2$ 爆炸递增。信息和格式在这套冗长的数据总线上不可避免地发生丢失乃至漂移。</p>
    </div>
  </div>
</div>

<!--
这个概率推倒是理工科学生绝对买单的东西。
非常震撼且直觉。
-->


---
layout: default
---

# 🧬 深入物理本质：Agent 熵与秩序

> 从宏观的热力学第二定律看待自动工作流的崩溃。

<div class="grid grid-cols-2 gap-8 my-8">
<div>
  <h3 class="text-red-300 font-bold mb-3 border-b border-slate-700 pb-2">编排复杂度：在制造系统熵</h3>
  <ul class="text-sm space-y-3 opacity-90 pl-4 list-disc marker:text-red-500">
    <li><b>环境熵：</b> UI界面突然弹个广告，原定按钮下移了一寸，Agent 直接点错乱序。</li>
    <li><b>传递熵：</b> Agent A 生成了输出文本交给 B，格式稍微没有对齐，B 彻底理解偏差。</li>
    <li><b>上下文熵：</b> 事情做到一半，Token 溢出，早期的重要约束"不可删除原文件"被遗弃出上下文窗口。</li>
  </ul>
</div>
<div class="bg-slate-900 p-6 rounded-lg text-center flex flex-col justify-center border border-slate-700 relative shadow-inner overflow-hidden">
  <div class="text-xs text-slate-400 mb-2 whitespace-nowrap text-left px-2">节点数与稳定性的战争</div>
  <div class="w-full flex mt-6 px-4">
    <!-- Success Line (Order) -->
    <div class="relative w-full h-[60px]">
      <div class="absolute font-mono text-[9px] text-[#00d2ff] opacity-80 bottom-full left-0 mb-1">系统成功率 / 秩序 (Order)</div>
      <!-- Gradient order bar representing decreasing success (starts wide/tall, shrinks) -->
      <div class="absolute bottom-0 left-0 bg-[#00d2ff] opacity-80 w-0 h-full origin-bottom-left transition-all duration-[2s]" v-click></div>
      <div class="absolute bottom-0 left-0 bg-gradient-to-r from-[#00d2ff] to-[#00d2ff]/10 h-full w-[25%]" style="clip-path: polygon(0 0, 100% 20%, 100% 100%, 0 100%);"></div>
      <div class="absolute bottom-0 left-[25%] bg-gradient-to-r from-[#00d2ff]/10 to-transparent h-full w-[75%]" style="clip-path: polygon(0 20%, 100% 95%, 100% 100%, 0 100%);"></div>
    </div>
  </div>
  <div class="w-full flex mt-2 px-4">
    <!-- Entropy Line (Chaos) -->
    <div class="relative w-full h-[60px]">
      <div class="absolute font-mono text-[9px] text-red-400 opacity-80 top-full left-0 mt-1">系统信息熵 / 混乱度 (Entropy)</div>
      <div class="absolute top-0 left-0 bg-gradient-to-r from-red-500/10 to-red-600 h-full w-[25%]" style="clip-path: polygon(0 100%, 100% 80%, 100% 0, 0 0);"></div>
      <div class="absolute top-0 left-[25%] bg-gradient-to-r from-red-600 to-red-900 h-full w-[75%]" style="clip-path: polygon(0 80%, 100% 5%, 100% 0, 0 0);"></div>
    </div>
  </div>
  <div class="absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2 bg-slate-800 text-white text-xs px-3 py-1 rounded border border-slate-600 shadow-xl opacity-90 z-20 font-mono tracking-wider items-center flex gap-2">
    编排节点增加 <carbon-arrow-right />
  </div>
</div>
</div>

<!--
这个可以看图说话，秩序被高节点编排给摧毁，系统不可避免走向混乱（即执行报错）。
-->

---
layout: center
---

# 那怎么办？就不用大管线了吗？
## 抗系统熵增的防御性设计

<div class="grid grid-cols-2 gap-8 mt-12 w-full max-w-4xl max-h-[80vh]">
  <div class="bg-slate-800/20 p-6 rounded-xl border border-slate-700">
    <div class="font-bold text-slate-200 text-base mb-3 flex items-center gap-2"><lucide-minus-circle class="w-5 h-5 opacity-70"/> 方略一：最小节点原则</div>
    <p class="text-sm opacity-70 mt-2 leading-relaxed">能使用基础通用模型解决的问题区间，坚决避免过分切割为微型专门处理链条。<br/><br/>构建原则：<b>新增调度节点的边际提效规模，如果不远超长链导致的传递衰减概率，果断丢弃合并。</b></p>
  </div>

  <div class="bg-slate-800/20 p-6 rounded-xl border border-slate-700">
    <div class="font-bold text-slate-200 text-base mb-3 flex items-center gap-2"><lucide-users class="w-5 h-5 opacity-70"/> 方略二：Human in the Loop</div>
    <p class="text-sm opacity-70 mt-2 leading-relaxed">为全自动架构留出人为断点控制截流层（例如 Antigravity 的 Planning 审查）。<br/><br/>在这个极易崩溃的发散机器管线中，人的核心价值不再是输出推理算力，而是提供<b>关键维度的方向审查拦截器。</b></p>
  </div>
</div>

---
layout: default
---

# 🔬 终极实证：自动科研框架 (AI for AI) 

如果编排达到极致，挑战整个 AI 科研周期全流程，系统论预言会应验吗？是的。

<div class="grid grid-cols-2 gap-8 mt-6">
  <div>
    <h3 class="font-bold text-xl text-yellow-300 mb-2 border-b border-slate-700 pb-2">科研全流程管道框架 FARS</h3>
    <div class="text-xs opacity-70 mb-4 px-2 py-1 bg-slate-800 inline-block border border-slate-600 rounded">日行迹智能科技出产。</div>
    <div class="flex items-center gap-1 text-[10px] w-full mt-4 font-mono">
      <div class="bg-blue-900/40 border border-blue-500/50 rounded py-2 px-1 flex-1 text-center truncate">Ideation<br/>构思假设</div>
      <carbon-arrow-right class="text-slate-500 shrink-0" />
      <div class="bg-blue-900/40 border border-blue-500/50 rounded py-2 px-1 flex-1 text-center truncate">Planning<br/>设计打样</div>
      <carbon-arrow-right class="text-slate-500 shrink-0" />
      <div class="bg-blue-900/40 border border-blue-500/50 rounded py-2 px-1 flex-1 text-center truncate">Experiment<br/>写码执行</div>
      <carbon-arrow-right class="text-slate-500 shrink-0" />
      <div class="bg-blue-900/40 border border-blue-500/50 rounded py-2 px-1 flex-1 text-center truncate">Writing<br/>撰写成文</div>
    </div>
    <div class="mt-8">
      <h3 class="font-bold text-xl text-cyan-300 mb-2 border-b border-slate-700 pb-2">Karpathy 的 AutoResearch</h3>
      <div class="text-sm opacity-80">前 OpenAI 联合创始人制作的个人版。</div>
    </div>
  </div>
  <div class="bg-slate-900 p-6 rounded-xl border border-slate-700 shadow-xl flex flex-col justify-center relative overflow-hidden">
    <div class="absolute -right-10 top-0 opacity-10 text-[10rem]">📜</div>
    <h3 class="text-xl font-bold mb-4 z-10 relative">💡 系统论的活生生印证：</h3>
    <p class="text-sm opacity-80 relative z-10 leading-relaxed mb-6">FARS 在运行中输出了<b>海量的 100 多篇“短论文”</b>，而不是万字长文、也不是顶级架构会议产出。</p>
    <div class="bg-green-900/20 border border-green-500/30 p-4 rounded-lg relative z-10">
      <p class="text-sm font-bold text-green-300 mb-2">这正是它之所以能跑通的秘密：</p>
      <p class="text-xs opacity-90 leading-relaxed">降低目标的纵深复杂度（短文） --> 大大减轻了 4 个 Agent 节点在每次接壤传递上的上下文丢失与约束崩溃概率 --> 单节点 P 上升 --> <span class="text-white bg-slate-800 px-1 border border-slate-600 rounded">P⁴ > 及格红线</span>，系统最终没有烂尾！</p>
    </div>
  </div>
</div>

<!--
FARS 产出的论文是 AI 评审系统打分的，超过了人类投稿者的平均得分。甚至可以读一下，让 AI 帮忙读。
-->

---
layout: center
---

# <lucide-shield-off class="inline-block mr-2 mb-1 opacity-70"/>物理机提权的底层安全矛盾

随着桌面智能代理走向极客主流，科研开发者必须面对难以绕开的权限架构隐患。

<div class="my-10 max-w-3xl mx-auto rounded-xl border border-slate-700 bg-slate-900/30 overflow-hidden shadow-lg p-8">
  <div class="text-center font-mono opacity-80 mb-6 text-xs tracking-wider uppercase">特权放大的边际危险</div>
  <div class="text-center">
    <p class="text-xl text-slate-200 leading-relaxed font-bold">
      当授予模型对操作系统的统筹操作上限不断抬高，<br/><span class="text-indigo-400 mt-3 inline-block">其由于幻觉反馈误触底层或造成数据级联灾难的风险系数将呈级数跃升。</span>
    </p>
  </div>
</div>

<div class="flex justify-center mt-12 gap-8 opacity-70 text-sm">
  <div class="flex items-center gap-2 border border-slate-700 bg-slate-800/50 px-4 py-2 rounded-lg font-mono text-xs"><lucide-lock class="w-4 h-4"/> 最小沙箱层封装</div>
  <div class="flex items-center gap-2 border border-slate-700 bg-slate-800/50 px-4 py-2 rounded-lg font-mono text-xs"><lucide-box class="w-4 h-4"/> 物理隔离 (Hypervisor)</div>
  <div class="flex items-center gap-2 border border-slate-700 bg-slate-800/50 px-4 py-2 rounded-lg font-mono text-xs"><lucide-scroll-text class="w-4 h-4"/> 全链路异步审计 (Audit Trails)</div>
</div>

<!--
收束第五章的高潮。
AI 学院的学生，安全防护和代理行为可控性（Alignment）是科研的热门发力点。这是一件好事。

前文铺垫埋下伏笔，科研让 AI 来，进展会让人类看不懂，科研是输出推动生产力发展的生产力，AI 科研在宏观程度上会有安全隐患。
-->
