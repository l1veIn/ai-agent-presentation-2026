# AI 工具链科研工作流分享 — 总览

## 核心叙事线

整个演讲围绕一条**能力跃迁曲线**展开，每一级跃迁都对应 AI 获得的新能力维度：

```
Web 对话式 AI → 工具调用 Agent → Computer Use 龙虾
   (语言能力)    (语言+工具能力)    (语言+工具+感官+执行)
    纯信道         闭环控制            操作系统级自治
```

### 三论穿插逻辑

| 跃迁阶段 | 对应理论 | 核心洞察 |
|---------|---------|---------|
| 对话式 AI | 信息论 | Prompt 是编码，AI 是信道，上下文窗口是信道容量 |
| 工具调用 Agent | 控制论 | 反馈回路质量决定协作上限，闭环优于开环 |
| Computer Use / 编排 | 系统论 | 复杂度雪崩——节点越多熵越大，交付成功率断崖下降 |

### 演进路线（贯穿全场的主线）

```
第二章            第三章+第四章              第五章
Web 对话 ──→ IDE AI / CLI Agent ──→ Computer Use 龙虾
              (带工具调用的 Agent)      (拥有电脑权限)
              Cursor / Antigravity     OpenClaw / WorkBuddy
              Claude Code / Codex      Anthropic Computer Use
              Gemini CLI               Microsoft Copilot Tasks
```

---

## 目标听众

- **人工智能学院研究生**
- 有编程基础，对 AI 原理有一定了解
- 目标：帮他们找到适合自己科研场景的 AI 工作流，而非盲目追新

## 演讲环境

- **演示平台**：macOS
- **网络环境**：4G 软路由网关（专页讲解）
- **预估时长**：60-90 分钟

## 文件索引

| 文件 | 内容 |
|------|------|
| [01_opening.md](./01_opening.md) | 第一章：开场 |
| [02_conversational_ai.md](./02_conversational_ai.md) | 第二章：对话式 AI + 信息论 |
| [03_ide_ai.md](./03_ide_ai.md) | 第三章：IDE 集成 AI + 控制论 |
| [04_cli_agent.md](./04_cli_agent.md) | 第四章：CLI Agent |
| [05_computer_use.md](./05_computer_use.md) | 第五章：Computer Use 龙虾 + 系统论（重头戏） |
| [06_vertical_tools.md](./06_vertical_tools.md) | 第六章：垂直工具 & 工作流设计 |
| [07_closing.md](./07_closing.md) | 第七章：收尾 |
| [style_guide.md](./style_guide.md) | 设计风格指南 |

## 待确认事项

> [!WARNING]
> 1. **演讲时长**：以上按 60-90 分钟设计，需要调整吗？
> 2. **实战演示**：现场真实操作还是预录视频？
> 3. **龙虾演示**：你本地有部署 OpenClaw 吗？还是用 WorkBuddy？
> 4. **网络准备页**：4G 软路由的品牌/型号？要讲到什么深度？
