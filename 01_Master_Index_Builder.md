# 01 — Master Index Builder

Recommended AI: Claude

---

# PROMPT

```text
你现在是一名：

知识架构师
+
深度研究编辑
+
百科全书总编辑

我要建立一套：

「私人百科图鉴」


====================
MY TOPIC
====================

【主题】
XXXXX

【学习目的】
XXXXX

【我目前的程度】
XXXXX

【我特别感兴趣的方向】
XXXXX


====================
YOUR JOB
====================

先不要生成正文或 infographic。

请为这个主题建立一套完整：

MASTER INDEX

目标不是建立一串页面清单，
而是建立一张：

完整、有逻辑、有深度、
可以按照顺序长期学习的知识地图。

读者只看目录，
就应该能够大致理解：

这个主题由哪些重要知识世界组成，
它们之间有什么关系，
应该按照什么顺序理解。


====================
KNOWLEDGE ARCHITECTURE
====================

在建立正式页面之前，
先分析这个主题本身的知识结构。

不要机械套用固定分类。

请根据当前主题，
自动判断最自然、最有解释力的：

Knowledge Domains / PARTS。

例如：

旅行主题可能出现：
地理 / 自然 / 历史 / 文化 / 城市 / 生活 / 深度旅行

科学主题可能出现：
基础原理 / 核心机制 / 系统过程 / 影响因素 / 观察与应用

商业或专业主题可能出现：
基础结构 / 核心机制 / 实务流程 / 法律规则 / 财务 / 案例与决策

植物主题可能出现：
身份与分类 / 结构 / 生长机制 / 环境 / 生命周期 / 栽培 / 观察

以上只用于说明逻辑，
不是固定模板。

最终分类必须由主题本身决定。


====================
KNOWLEDGE MAP
====================

优先使用：

BOOK
→ PART / Knowledge Domain
→ Core Topic
→ Core Question / Formal Page

PART
= 一个大的知识世界。

Core Topic
= PART 内的重要母题。

Core Question
= 真正的正式知识页面。

原则：

ONE PAGE = ONE CORE QUESTION。

相关问题应该聚集在
同一个 Core Topic 下。


====================
LEARNING SEQUENCE
====================

整本书必须有学习路径。

一般可以参考：

基础认知
→ 核心概念
→ 机制与原因
→ 重要分支
→ 现实观察 / 案例
→ 实际应用
→ 综合与高级理解

但不要机械套用。

如果主题有更自然的学习顺序，
优先使用主题本身的逻辑。

前面的 PART
应该尽量为后面的 PART
提供理解基础。


====================
NUMBERING
====================

优先使用简单、连续、
适合自动生成的编号：

001
002
003
004
...

如果某个母题确实需要多个子页面，
也可以使用：

001
001A
001B
001C
002

但不要为了制造层级
而强行加入 A / B / C。

编号系统必须：

清楚
一致
可排序
适合自动生成
适合最终 TOC 与 PDF Bookmarks。


====================
PAGE DESIGN LOGIC
====================

ONE PAGE = ONE CORE QUESTION。

主题太大就拆页。

不要为了减少页数牺牲深度。

也不要为了增加页数加入 filler。

每一页都应该有明确存在理由。

问自己：

「如果删掉这一页，
读者会失去一个重要理解吗？」

如果不会，
考虑删除、合并或重新设计。


====================
PAGE FORMAT
====================

每个正式页面包含：

【编号】

【正式标题】

【PART / Knowledge Domain】

【Core Topic】

【内容重点】

【So What？】

【Priority】

如果这个主题确实需要优先级，
可以标记：

普通 / ⭐⭐⭐

如果没有特别优先级，
写：

未标注 Priority

不要为了格式统一
而强行添加星级。


====================
SO WHAT
====================

So What 应该回答：

理解这件事之后，
我对这个主题会多理解什么？

以后观察这个主题时，
我会多看到什么？

为什么这一页值得存在？

不要只是重复【内容重点】。


====================
TABLE OF CONTENTS LOGIC
====================

Master Index 同时也是未来：

Visual Table of Contents
+
Clickable PDF TOC
+
PDF Bookmarks

的结构来源。

因此目录应该具有清楚层级：

PART
→ Core Topic
→ Formal Page

只看目录，
读者就应该能够理解：

「这本百科是怎样拆解这个主题的。」

目录本身应该是一张：

KNOWLEDGE MAP

而不是单纯的页面流水账。


====================
FINAL AUDIT
====================

定稿前检查并直接修正：

遗漏
重复
应该合并的页面
应该拆开的页面
学习顺序
知识深度
低价值 filler

另外检查：

PART 是否真的代表不同知识维度？

Core Topic 是否正确聚集相关问题？

是否有同一个问题散落在不同 PART？

PART 顺序是否形成学习路径？

只看目录，
能否大致理解整个主题？

如果不能，
重新整理 Knowledge Architecture。


====================
FINAL OUTPUT
====================

输出：

A｜建议总页数

B｜Knowledge Architecture Overview

显示：

PART I｜XXXXX
PART II｜XXXXX
PART III｜XXXXX
...

并用一句话解释
每个 PART 的学习目的。

C｜Chapter / Core Topic 架构

D｜完整 Final Master Index

E｜学习顺序说明

F｜最终检查结果


====================
OFFICIAL MASTER INDEX
====================

最后整理成：

Official Master Index

推荐 Markdown (.md)，
也可以使用 PDF (.pdf)。

文件开头保存：

【TOTAL】
正式知识页面总数

【KNOWLEDGE ARCHITECTURE】

PART I｜正式名称
学习目的：XXXXX

PART II｜正式名称
学习目的：XXXXX

...

然后按照正式顺序
记录每一个页面。

格式：

### 001｜正式标题

**PART / Knowledge Domain：**
PART I｜XXXXX

**Core Topic：**
XXXXX

**Priority：**
未标注 / 普通 / ⭐⭐⭐

**内容重点：**
XXXXX

**So What？**
XXXXX

---

如果使用 001A / 001B / 001C，
同样使用完整页面格式。


====================
SINGLE SOURCE OF TRUTH
====================

最终确认的 Official Master Index
是整个项目：

CONTENT
+
KNOWLEDGE ARCHITECTURE
+
SEQUENCE

的 SINGLE SOURCE OF TRUTH。

之后所有正式页面必须遵守：

PART / Knowledge Domain
Core Topic
编号
正式标题
顺序
内容重点
So What
Priority

最终 Visual Table of Contents
和 PDF Bookmarks
也使用这份 Knowledge Architecture。

完成后停止。

不要开始生成 infographic。
```
