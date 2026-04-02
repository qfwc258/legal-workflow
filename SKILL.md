---
name: legal-workflow
description: 律师工作流工具 - 整合法律文书生成、合同审查、诉讼可视化、法律援助文档四大核心功能
version: 1.0.0
author: qfwc258
---

# 法律工作流 (Legal Workflow)

律师一站式AI助手，整合法律文书生成、合同审查、诉讼可视化、法律援助文档四大核心功能。

## 功能模块

### 1. 法律文书生成 (Legal Document)
- 双驱动模式：关键词匹配 + AI案情解析
- 内置200+官方权威模板
- 覆盖民事、商事、刑事等9大领域67类场景
- 合规校验、法条关联、多格式导出

**触发场景**：起诉状、答辩状、合同协议、申请书、判决书等

### 2. 合同审查 (Contract Review)
- 三层审查：基础审查、业务审查、法律审查
- 标注式审查（仅添加注释，不修改原文）
- 生成审核报告、业务流程图
- 风险等级评估

**触发场景**：合同审核、条款分析、风险评估

### 3. 诉讼可视化 (Litigation Visualization)
- 诉讼时间轴图谱生成
- 关键法律事实节点提取
- 支持HTML/图片多格式输出
- A4打印优化

**触发场景**：诉讼时间线、案件 chronology、庭审提纲

### 4. 法律援助文档 (Legal Aid)
- 批量填充Word模板
- 保持原文档格式
- 支持自定义占位符
- 多模板同时处理

**触发场景**：法援结案、阅卷笔录、代理意见

## 目录结构

```
legal-workflow/
├── SKILL.md              # 本文件
├── _meta.json            # 元数据
├── user_preferences.json # 用户偏好配置
├── memory/               # 记忆存储
│   └── word_format_memory.md
├── references/           # 参考文档
│   ├── word_format_standard.md  # Word公文格式规范
│   ├── templates.md             # 模板指南
│   ├── legal_codes.md          # 法条关联
│   └── format_standards.md     # 格式规范
├── scripts/              # 核心脚本
│   ├── document_generator.py    # 文书生成
│   ├── contract_analyzer.py    # 合同审查
│   ├── timeline_generator.py    # 时间轴生成
│   └── legal_aid_filler.py     # 法援填充
└── toolkit/              # 工具集
    └── templates/               # 内置模板
```

## 依赖安装

```bash
pip install python-docx==0.8.11 reportlab==3.6.12 jieba==0.42.1 fuzzywuzzy==0.18.0 python-Levenshtein==0.21.1
```

## 使用示例

### 生成法律文书
```
用户：帮我写一份借款纠纷的民事起诉状
助手：[调用legal-document模块]

### 生成合同审查报告
用户：审查这份采购合同
助手：[调用contract-review模块]

### 创建诉讼时间轴
用户：帮我做一个诉讼时间轴
助手：[调用litigation-viz模块]

### 批量生成法援文书
用户：根据元素文件填充法援模板
助手：[调用legal-aid模块]
```

## 输出规范

| 模块 | 输出格式 | 命名规则 |
|------|----------|----------|
| 文书生成 | .docx | {文书类型}_{案号}.docx |
| 合同审查 | .docx + .html | 审核结果：{合同名}/ |
| 可视化 | .html | {案件名}-诉讼时间轴图谱.html |
| 法援文档 | .docx | {模板名}_填写版.docx |

## 律师信息配置

首次使用请配置律师署名信息：
- 姓名：陈伟律师
- 律所：湖南金厚（宁乡）律师事务所
- 电话：13975892485

## Word文档格式

遵循 GB/T 9704-2012 公文格式标准，详见 `references/word_format_standard.md`