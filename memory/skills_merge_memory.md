# Agent Memory - 技能配置

## 记忆类型: 事实 (Fact)

**更新内容**: legal-ppt-template 已合并至 pptx-generator

**合并时间**: 2026-04-02

---

## 合并后的 pptx-generator 技能

**路径**: `d:\trae\.trae\skills\pptx-generator`

**包含功能**:
1. PptxGenJS 从零创建PPT
2. XML编辑现有模板
3. 文本提取 (markitdown)
4. **法律案件分析模板（已合并）**

---

## 法律主题配色 (Legal Theme)

```javascript
const legalTheme = {
  primary: "1E3A5F",    // 深海军蓝 - 标题
  secondary: "2C5282",  // 中蓝 - 副标题
  accent: "C9A227",      // 金色点缀 - 高亮
  light: "E8D48A",       // 浅金
  bg: "FFFFFF"           // 白色背景
};
```

---

## 法律幻灯片模式

| 模式 | 用途 |
|------|------|
| Case Overview | 交替背景表格展示当事人信息 |
| Claims | 左侧编号卡片 + 右侧内容 |
| Defense Points | 左侧彩色竖条 + 右侧内容 |
| Key Issues | 三栏卡片布局 |
| Evidence List | 三列分类证据清单 |

---

## 12页案件分析模板结构

| 页码 | 类型 | 内容 |
|------|------|------|
| 1 | 封面 | 案件标题、案号、法院 |
| 2 | 概述 | 当事人信息、案件背景 |
| 3 | 时间轴 | 案件发展脉络 |
| 4 | SWOT | 双方优劣势分析 |
| 5 | 法律要件 | 构成要件分解 |
| 6 | 金额计算 | 诉请金额明细 |
| 7 | 诉讼进度 | 阶段性进度 |
| 8 | 核心策略 | 主要诉求 |
| 9 | 抗辩分析 | 对方抗辩+反驳 |
| 10 | 证据清单 | 三栏分类证据 |
| 11 | 法律依据 | 法条引用 |
| 12 | 结尾 | 谢谢页+联系方式 |

---

## 废弃技能

- `legal-ppt-template` - 已合并至 pptx-generator

---

## 相关文件

- SKILL.md: `d:\trae\.trae\skills\pptx-generator\SKILL.md`
- brand_vi.js: `d:\trae\.trae\skills\pptx-generator\brand_vi.js`
- 律所VI: 湖南金厚（宁乡）律师事务所, 139 7589 2485

---

## GitHub仓库

- trae-skills: https://github.com/qfwc258/trae-skills
  - skills/pptx-generator/SKILL.md
  - skills/pptx-generator/brand_vi.js