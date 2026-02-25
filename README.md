# LLM记忆仓库

> 🧠 为您的LLM对话建立长期记忆系统

这是一个专门用于存储和管理您与LLM助手对话历史的知识库。每次对话都会被系统性地记录、分类和索引，形成您的个人AI记忆网络。

## 📁 仓库结构

```
llm-memory-warehouse/
├── conversations/     # 每次对话的记忆卡片
├── knowledge/         # 提取的知识点和概念
├── references/        # 参考资料和链接
├── prompts/           # 管理Prompt模板
├── templates/         # 文件模板
└── README.md          # 本说明文件
```

## 🚀 使用流程

### 1. 对话记录自动化
- 每次对话结束后，系统会自动生成记忆卡片
- 文件命名格式：`YYYY-MM-DD-主题描述.md`
- 存储位置：`conversations/` 目录

### 2. 知识提取
- 从对话中识别重要知识点
- 存储位置：`knowledge/` 目录
- 命名规范：`主题-知识点.md`

### 3. 参考管理
- 记录对话中提到的参考资料、链接、文档
- 存储位置：`references/` 目录

## 📝 记忆卡片模板

使用 `templates/memory-card-template.md` 作为标准格式，确保信息结构化和可检索。

## 🤖 自动化Prompt

`prompts/memory-updater-prompt.md` 包含了完整的记忆更新指令，指导AI如何处理每次对话的记忆记录。

## 🔗 仓库链接
- GitHub仓库：https://github.com/bladepipe/llm-memory-warehouse
- 最新更新时间：2026-02-25

> 💡 提示：您可以随时访问此仓库查看、搜索和管理您的所有AI对话记忆！