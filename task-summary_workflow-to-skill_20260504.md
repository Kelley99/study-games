# Workflow-to-Skill 规则添加 - 2026-05-04

## 任务
为灵超、代可行、文慧、大宏四个 agent 添加永久规则：完成完整工作流程后生成技能。

## 执行结果

### 已更新文件
| Agent | 文件路径 | 状态 |
|-------|---------|------|
| 灵超 | `/Users/kelley/.qclaw/workspace/AGENTS.md` | ✅ |
| 代可行 | `/Users/kelley/.qclaw/workspace-agent-29b6e205/AGENTS.md` | ✅ |
| 文慧 | `/Users/kelley/.qclaw/workspace-agent-reading/AGENTS.md` | ✅ |
| 大宏 | `/Users/kelley/.qclaw/workspace-agent-finance/AGENTS.md` | ✅ |

### 添加的规则内容

```markdown
## 🎯 Workflow-to-Skill Rule (Permanent)

**When a complete workflow is successfully executed, generate a skill to capture it.**

This is a permanent memory command. After completing any non-trivial, reusable workflow:

1. **Identify** — Was this workflow complex enough to benefit future reuse?
2. **Document** — If yes, create a skill file capturing:
   - Workflow steps
   - Key decisions and rationale
   - Tools/commands used
   - Edge cases and gotchas
   - Example usage
3. **Store** — Save to `skills/` directory or appropriate location
4. **Reference** — Update relevant memory files to note the skill exists

**Why**: Workflows are expensive to rediscover. A skill makes the knowledge permanent and shareable across sessions and agents.

**Examples of workflow-to-skill candidates**:
- Multi-step debugging processes
- Deployment pipelines
- Data processing workflows
- Content creation workflows
- Integration setups

**Not every task needs a skill** — use judgment. Simple one-off tasks don't need capture. Reusable, multi-step workflows do.
```

## 意义
- 工作流程知识不再随会话结束而丢失
- 技能可跨会话、跨 agent 共享
- 减少重复探索成本

## 备注
这是永久性命令，已写入各 agent 的 AGENTS.md 核心规则文件。
