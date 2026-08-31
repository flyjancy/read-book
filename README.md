# Read Book

**完整阅读技术或非虚构书籍并生成结构化中文总结的 Codex skill**<br>
**A Codex skill for reading complete technical or nonfiction books and producing structured Chinese summaries**

[中文](#中文) · [English](#english)

---

## 中文

Read Book 从网页链接或本地文件完整阅读技术及非虚构书籍，并生成基于全书内容的结构化中文总结。它会先核对书目信息和来源，再按目录逐章覆盖正文，同时检查影响结论的图表、注释与附录。

该 skill 不适用于学术论文、小说，也不会复制外部托管的受版权保护书籍全文。

### 核心能力

| 能力 | 作用 |
| --- | --- |
| 全书覆盖 | 先扫描目录，再逐章阅读并核对覆盖范围 |
| 多种来源 | 支持可访问的网页链接和本地文件 |
| 图表核对 | 检查影响结论的图、表、图例、注释和附录 |
| 结构化总结 | 输出核心命题、逐章摘要、关键概念、证据背景和个人点评 |
| 观点分层 | 区分作者主张、书中证据、历史背景与个人分析 |
| 版权约束 | 对受版权保护的外部书籍只保留原创总结和必要短引文 |

### 快速开始

克隆到 Codex skills 目录：

```bash
git clone https://github.com/flyjancy/read-book.git ~/.codex/skills/read-book
```

在 Codex 中提供书籍链接或本地文件：

```text
使用 $read-book 阅读并总结这本书：https://example.com/book
```

默认结果直接返回到对话中。只有明确要求保存时，才会创建 Markdown 文件。

### 默认输出

- 基本信息与来源说明
- 一句话总结与全书核心命题
- 逐章摘要
- 关键概念、常见误读、证据与历史背景
- 今天仍适用及需要谨慎使用的内容
- 个人点评，以及适用时的实践清单

---

## English

Read Book reads complete technical or nonfiction books from accessible web links or local files and produces structured Chinese summaries grounded in the full text. It verifies bibliographic information and sources, follows the table of contents chapter by chapter, and checks figures, tables, notes, and appendices that affect the conclusions.

This skill is not intended for academic papers or fiction, and it does not reproduce externally hosted copyrighted books.

### What It Provides

| Capability | Purpose |
| --- | --- |
| Full-book coverage | Scan the contents, read every chapter, and track coverage |
| Multiple sources | Work with accessible web links and local files |
| Visual inspection | Check relevant figures, tables, legends, notes, and appendices |
| Structured summaries | Cover theses, chapters, concepts, evidence, context, and commentary |
| Clear attribution | Separate the author's claims, supporting evidence, historical context, and analysis |
| Copyright safeguards | Keep only original summaries and necessary short quotations for protected external books |

### Quick Start

Clone the skill into your Codex skills directory:

```bash
git clone https://github.com/flyjancy/read-book.git ~/.codex/skills/read-book
```

Then give Codex a book URL or local file:

```text
Use $read-book to read and summarize this book: https://example.com/book
```

By default, the summary is returned in the conversation. A Markdown file is created only when explicitly requested.

### Default Output

- Bibliographic details and source notes
- A one-sentence summary and the book's central theses
- Chapter-by-chapter summaries
- Key concepts, common misreadings, evidence, and historical context
- What remains useful today and what requires caution or updating
- Commentary and, when appropriate, a practical checklist
