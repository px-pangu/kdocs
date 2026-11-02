# 金山文档 / WPS 云文档 · Kdocs CLI Skill

> 操作金山文档（WPS 云文档 / Kdocs）云文档：新建、读取、编辑、搜索、分享，覆盖智能文档、表格、PDF、PPT 与知识库

![Type](https://img.shields.io/badge/type-Agent%20Skill-4a6b7c)
![Upstream](https://img.shields.io/badge/upstream-kdocs%20v2.5.7%20-%20金山文档官方%20Skill-8f8a80)
![License](https://img.shields.io/badge/license-归原作者-b8935a)

> ⚠️ 本仓库是个人使用环境中的 Skill 归档副本，**版权归原提供方**：kdocs v2.5.7 · 金山文档官方 Skill

## 这是什么

金山文档官方提供的 CLI Skill，让你在对话里直接操作云端文档：写周报、建报名表、把接龙转成表格、把网页存进文档、文档转 Markdown、表格美化、知识库归档。

## 能力范围

| 域 | 能做什么 |
|---|---|
| 文档 | 新建、读取、编辑、搜索、分享、回收站还原 |
| 表格 | 在线表格、智能表格、多维表格读写；表格美化；接龙转表格 |
| 演示 | AI PPT 生成、演示文稿读写 |
| PDF | 拆分、导出、转换 |
| 知识库 | 标签分类、归档、收藏管理、碎片笔记整理 |

支持格式：智能文档、Word、Excel、PDF、PPT、智能表格、多维表格。

## 前期准备

```bash
# 1. 安装 CLI（按 SKILL.md 的「工具安装与认证」一节）
# 2. 完成登录认证
# 3. 验证
kdocs --version
```

认证凭据保存在本机，**不进仓库**。

## 调用方式

在对话里直接说要做的事即可，例如：

```
把这段接龙内容整理成表格，存到我的金山文档
把这个网页剪藏到知识库，打上「产品」标签
把这份周报导出成 PDF
```

## 目录结构

```
kdocs/
├─ SKILL.md      严格规则 · 安装认证 · 调用格式 · 能力范围 · 错误速查
├─ scripts/      CLI 封装与批处理脚本
└─ references/   接口与字段参考
```

## 许可

该 Skill 由金山文档官方提供，著作权归原提供方所有。本仓库仅为个人归档，**不作出任何再许可**，详见 `NOTICE.md`。


## 安装

```bash
git clone https://github.com/px-pangu/kdocs.git ~/.workbuddy/skills/kdocs
# Claude Code：~/.claude/skills/kdocs
```

> 若原包依赖 CLI（如 `kdocs`、`ima`、`wecom`、`pdfkit`），需先按 `SKILL.md` 的安装与认证段落配置本机环境。**仓库内不含任何凭据。**

