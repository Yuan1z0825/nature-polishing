# Nature-Style Academic Polishing Skill

一个基于 Nature 正刊论文写作风格分析与科学英语写作课程构建的学术润色 skill，可将中文学术草稿转化为符合 Nature 期刊标准的英文学术文本。

## 数据来源

从本目录下 18 篇 Nature 正刊论文（s41586 系列，2026 年发表）中抽样精读 5 篇，并系统学习一门科学英语写作课程，提取以下风格特征与写作规范：

- 沙漏结构（Hourglass：broad → narrow → broad）
- 写作顺序 ≠ 阅读顺序（作者逻辑 vs 读者逻辑）
- Introduction 的 4 个必答问题与 2 个禁区
- Results（过去时 + 定量）与 Discussion（hedging + 机制）的语言区分
- Methods 写作的 7 个禁用模糊短语
- 标题"好奇心 + 可信度"原则（≤75 字符）
- 摘要 mini-paper 五步模板
- 结论三段式（贡献 → 证据 → 边界）
- 四种引用类型（支撑 / 借用 / 对比 / 复用）
- 一手来源与二手来源的引用原则
- 模糊语（hedging）的三级校准
- 弱动词替换策略
- 英式拼写、冠词使用、缩写规范
- 过度声明（overclaim）检测
- 校订自查清单
- AI 使用红绿灯模型

## 核心能力

| 能力 | 说明 |
|------|------|
| 长句拆分 | 中文 >40 字符或多逗号句子自动拆为 2-3 个英文短句，每句 ≤30 词 |
| 分区润色 | 根据段落所属章节（Intro / Results / Discussion / Methods / Abstract）自动应用对应规则 |
| 时态控制 | Results = 过去时 + 定量细节；Discussion = hedging + 因果/泛化/局限 |
| 词汇升级 | 弱动词 / 模糊形容词替换为精确学术用语 |
| 模糊语校准 | 按证据强度匹配用词（demonstrate → suggest → may reflect） |
| 结构重组 | 摘要 / 引言 / 结论按 Nature 标准模板对齐 |
| 标题优化 | 去除技术术语，保证可检索性，控制长度 |
| 引用规范 | 检查一手 / 二手来源，避免 straw man 式贬低前人工作 |
| 过度声明检测 | 标记绝对化措辞、因果跳跃、范围扩张 |
| 即贴即用 | 输出为纯文本，可直接复制粘贴到论文草稿中 |

## 使用方法

让 Claude 执行以下任意一种指令即可触发：

- "用 nature-polishing 润色这段文字"
- "把这段话改成 Nature 风格"
- "polish this in Nature style"

## 文件结构

```
.claude/skills/nature-polishing/
  SKILL.md          — skill 指令定义（25 条规则 + 12 步工作流）
  README.md         — 使用说明
```

## 适用场景
<img width="1730" height="924" alt="image" src="https://github.com/user-attachments/assets/2137d663-8e8e-426c-9fa9-210302022443" />

- 中文学术草稿的英文翻译与润色
- 已有英文文本的 Nature 风格改写
- 摘要、引言、结论、Results、Discussion、Methods 段落的结构优化
- 论文返修时的语言升级
- 标题与摘要的重新起草

## 不适用场景

- 完整论文从零起草（应参考具体期刊的 author guidelines）
- 非学术类写作（科普、博客、新闻报道等）
- 需要保留原文特定术语或作者个人风格的情况
