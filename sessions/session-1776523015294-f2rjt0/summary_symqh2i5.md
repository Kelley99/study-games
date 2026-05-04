## 任务背景
为灵超、代可行、文慧、大宏四个agent添加永久记忆命令：完成完整工作流程后生成技能文件。

## 执行过程
1. 读取四个agent的AGENTS.md文件路径
2. 编写Workflow-to-Skill规则（非平凡、可复用工作流程捕获标准）
3. 逐个更新：灵超→代可行→文慧→大宏的AGENTS.md
4. 创建任务文档task-summary_workflow-to-skill_20260504.md
5. 更新memory/2026-05-04.md记录工作内容

## 关键结果
- **更新文件**：4个AGENTS.md全部更新
  - /Users/kelley/.qclaw/workspace/AGENTS.md（灵超）
  - /Users/kelley/.qclaw/workspace-agent-29b6e205/AGENTS.md（代可行）
  - /Users/kelley/.qclaw/workspace-agent-reading/AGENTS.md（文慧）
  - /Users/kelley/.qclaw/workspace-agent-finance/AGENTS.md（大宏）
- **规则要点**：捕获步骤/决策/工具/边缘情况/示例，存储skills/目录
- **Artifact**：task-summary_workflow-to-skill_20260504.md

## 结论建议
工作流程知识不再随会话结束丢失。简单一次性任务无需捕获，多步骤可复用流程必须生成技能。建议各agent在完成复杂任务后主动识别并创建技能文件。