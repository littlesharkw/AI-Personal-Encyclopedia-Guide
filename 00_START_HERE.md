# 00 — START HERE

这套系统分成四个阶段。

有一个重要原则：

**先准备并上传当前步骤需要的文件，再发送 Prompt。**

如果文件已经在当前对话中可用，
不需要重复上传。

---

## STEP 1 — BUILD THE KNOWLEDGE MAP

推荐 AI：

**Claude**

这一步不需要上传任何文件。

打开：

`01_Master_Index_Builder.md`

复制里面的 Prompt，
填写：

- 主题
- 学习目的
- 当前程度
- 特别感兴趣的方向

然后发送给 Claude。

完成后得到：

**Official Master Index**

它是之后：

**内容 + 知识架构 + 顺序**

的唯一权威。

### USER ACTION

完成后，

请把最终确认版本手动保存为：

**Official Master Index**

推荐 `.md`。

`.pdf` 也可以。

下一步需要把这个文件上传到 ChatGPT。

---

## STEP 2 — BUILD THE VISUAL SYSTEM

推荐 AI：

**ChatGPT**

### BEFORE SENDING THE PROMPT

先打开一个 ChatGPT 对话。

手动上传：

**Official Master Index**

确认文件已经出现在当前对话中。

然后打开：

`02_Visual_Style_Setup.md`

复制并发送里面的 Prompt。

### WHAT HAPPENS NEXT

ChatGPT 会逐张建立：

**Visual Style Test**

每次只测试一张。

你可以：

修改当前 Test Page

或

要求继续下一个 Visual Test。

当你确认喜欢的视觉方向后，

ChatGPT 会建立：

**Official Visual Style Lock**

并输出为 PDF。

实际文件名必须包含主题名称。

例如：

```text
Iceland_Official_Visual_Style_Lock.pdf
Sleep_Official_Visual_Style_Lock.pdf
Dahlia_Official_Visual_Style_Lock.pdf
```

### USER ACTION

下载并保存这份 PDF。

之后流程中，
无论实际文件名是什么，

都统一称它为：

**Official Visual Style Lock**

Visual Style Test
不属于正式图鉴页面。

---

## STEP 3 — START PRODUCTION

推荐 AI：

**ChatGPT**

建议打开一个新的 ChatGPT 对话。

### BEFORE SENDING THE PROMPT

手动上传：

① **Official Master Index**

② **Official Visual Style Lock**

确认两个文件
都已经出现在当前对话中。

然后打开：

`03_Hourly_Auto_Generator.md`

复制并发送里面的 Prompt。

### FIRST RUN

第一次运行：

```text
Setup
↓
Read Official Files
↓
Generate First Formal Page
↓
Validate
↓
Create Scheduled Task
```

第一张正式页面
必须重新从 Official Master Index
第一个正式页面开始。

Visual Style Test
不计算在正式进度内。

### SCHEDULED PRODUCTION

之后：

**ONE SCHEDULED RUN = ONE PAGE**

Scheduled Task 会按照
Official Master Index
的实际顺序继续生成。

不需要每小时重新上传文件
或重新发送 03 Prompt。

但仍建议偶尔检查：

生成有没有停止

有没有跳页或重复

内容有没有偏离 Master Index

视觉有没有偏离 Style Lock

---

## STEP 4 — BUILD THE FINAL BOOK

所有正式页面完成后，

使用：

`04_Final_Audit_and_PDF.md`

### BEFORE SENDING PROMPT 1

确保当前 ChatGPT
可以访问：

① **Official Master Index**

② **Official Visual Style Lock**

③ **全部正式图鉴页面**

如果这些文件已经在当前对话中可用，
不需要重复上传。

如果不在，
先手动上传或提供给当前对话。

然后发送：

**PROMPT 1 — DESIGN THE BOOK**

### BOOK DESIGN

ChatGPT 会参考：

Official Master Index

和：

Official Visual Style Lock

设计：

**Cover + Complete TOC**

并给出每一张
封面／目录图的独立生图指令。

按照这些指令：

逐张生成
↓
检查
↓
修改
↓
确认

### BEFORE SENDING PROMPT 2

确认 ChatGPT 可以访问：

全部正式图鉴页面

+
最终确认的 Cover

+
最终确认的 TOC

然后发送：

**PROMPT 2 — BUILD THE FINAL PDF**

最后建立：

**Final PDF**

包括：

Clickable TOC
+
PDF Metadata

---

## THE TWO OFFICIAL FILES

整个生产流程围绕：

```text
Official Master Index
+
Official Visual Style Lock
```

运行。

简单来说：

```text
01
CREATE THE MASTER INDEX
↓
SAVE IT

02
UPLOAD MASTER INDEX
↓
SEND PROMPT
↓
CREATE STYLE LOCK
↓
SAVE IT

03
UPLOAD BOTH OFFICIAL FILES
↓
SEND PROMPT
↓
START AUTOMATION

04
MAKE SURE ALL BOOK ASSETS ARE AVAILABLE
↓
SEND DESIGN PROMPT
↓
APPROVE COVER + TOC
↓
SEND PDF PROMPT
```

---

## START

现在打开：

`01_Master_Index_Builder.md`
