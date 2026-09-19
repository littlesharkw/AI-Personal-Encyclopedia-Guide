# 03 — Hourly Auto Infographic Generator

Recommended AI: ChatGPT

> FIRST RUN = SETUP + FIRST PAGE  
> SCHEDULED RUN = ONE PAGE

---

## BEFORE YOU START

建议打开一个新的 ChatGPT 对话。

手动上传：

① **Official Master Index**  
② **Official Visual Style Lock**

确认两个文件都已经在当前对话中可用后，
再发送下面的 Prompt。

第一次设置完成后，
不需要在每次 Scheduled Run 前重新上传文件。

# PROMPT

```text
现在进入自动生成阶段。

使用：

① Official Master Index
② Official Visual Style Lock


====================
SOURCE OF TRUTH
====================

Official Master Index
=
编号、正式标题、实际顺序、
内容重点、So What、Priority
的唯一权威。

Official Visual Style Lock
=
视觉的唯一权威。

不得：

改题
跳页
重复
增加主题
自行重新设计视觉风格

页面顺序必须按照
Official Master Index
的实际顺序读取。

不得根据编号自行推算。


====================
PHASE A｜SETUP — RUN ONCE
====================

PHASE A
只在当前 ChatGPT 对话
第一次运行一次。

读取：

Official Master Index
Official Visual Style Lock

建立初始状态：

【TOTAL】
读取正式页面总数

【已完成】
无；正式进度 0 / TOTAL

【CURRENT】
Official Master Index
第一个正式页面：

编号｜正式标题

并读取完整：

CURRENT 内容重点
CURRENT So What
CURRENT Priority

【NEXT】
按照 Master Index 实际顺序
读取下一个正式页面

【NEXT+1】
按照 Master Index 实际顺序
读取再下一个正式页面

同时读取并保存完整：

VISUAL STYLE LOCK

Visual Style 测试页面
不属于正式生成进度。

初始化时：

【已完成】
无；正式进度 0 / TOTAL

正式生产必须从
Official Master Index
第一个正式页面开始。


====================
GENERATE FIRST PAGE
====================

初始化完成后，

立即在当前 ChatGPT 对话
生成 CURRENT。

使用：

CURRENT
CURRENT 内容重点
CURRENT So What
CURRENT Priority
VISUAL STYLE LOCK

生成 ONE PAGE。

生成后核对：

编号
正式标题
Priority / 固定信息
视觉风格

如果不正确：

不要推进状态，
继续处理同一 CURRENT。

如果正确：

标记 CURRENT 已完成。


====================
PREPARE SCHEDULED TASK
====================

第一张验证成功后：

CURRENT → 已完成
NEXT → CURRENT
NEXT+1 → NEXT

然后按照 Official Master Index
的实际顺序读取并保存：

新的 CURRENT 内容重点
新的 CURRENT So What
新的 CURRENT Priority
新的 NEXT+1

同时更新正式进度。

然后创建 Scheduled Task。

Scheduled Task 从更新后的 CURRENT 开始，
也就是从第二个正式页面开始。

创建 Scheduled Task 时：

不要把 PHASE A 写入 Scheduled Task Prompt。

Scheduled Task Prompt
只保存下面的：

PHASE B｜SCHEDULED TASK PROMPT

并填入刚刚准备好的最新状态。


====================
PHASE B｜SCHEDULED TASK PROMPT
====================

以下内容才是 Scheduled Task
以后每次运行使用的 Prompt：


--------------------
CURRENT STATE
--------------------

【TOTAL】
保存 TOTAL

【已完成】
保存正式进度

【CURRENT】
保存当前编号｜正式标题

【CURRENT 内容重点】
保存完整内容重点

【CURRENT So What】
保存完整 So What

【CURRENT Priority】
从 Official Master Index 原样保存

【NEXT】
保存下一个正式页面

【NEXT+1】
保存再下一个正式页面


--------------------
VISUAL STYLE LOCK
--------------------

保存完整的
Official Visual Style Lock 执行规则。

整个正式生产阶段保持不变。


--------------------
GENERATE
--------------------

每轮只生成 CURRENT。

直接使用已经保存的：

CURRENT
CURRENT 内容重点
CURRENT So What
CURRENT Priority
VISUAL STYLE LOCK

生成 ONE PAGE。

生成后核对：

编号
正式标题
Priority / 固定信息
视觉风格

正确才算完成。

如果不正确：

保持 CURRENT 不变。


--------------------
ADVANCE
--------------------

成功后必须实际更新 Scheduled Task Prompt：

CURRENT → 已完成
NEXT → CURRENT
NEXT+1 → NEXT

然后从 Official Master Index
按照实际顺序读取并保存：

新的 CURRENT 内容重点
新的 CURRENT So What
新的 CURRENT Priority
新的 NEXT+1

并更新正式进度。

VISUAL STYLE LOCK 保持不变。

不得只在报告文字中声称已推进。


--------------------
REPORT
--------------------

成功后只显示：

已完成：编号｜正式标题
当前进度：X / TOTAL
下一张：更新后的 CURRENT 编号｜正式标题

NEXT+1 属于内部状态，
不需要显示。


--------------------
FINISH
--------------------

完成 Official Master Index
最后一个正式页面后停止。

不得创造新页面。

只报告：

整套图鉴已完成。
最终进度：TOTAL / TOTAL

然后进入：

04_Final_Audit_and_PDF.md
```
