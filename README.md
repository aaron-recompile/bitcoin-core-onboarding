# Bitcoin Core Onboarding Notes / 比特币核心开发者入门笔记

Author: Aaron Zhang  
Repo: `bitcoin-core-onboarding`

---

## 1. What this repo is about / 本仓库的定位

This repository is my long-term reading and thinking log while onboarding to **Bitcoin Core** as a developer.

It is **not** an official guide, but a curated and opinionated collection of:

- Original articles, talks, and resources about Bitcoin Core onboarding  
- My **faithful Chinese translations** of selected texts  
- My own **commentary and technical notes** as a developer  
- Structured **learning maps** extracted from each article

The goal:

> To build a reusable, high-signal knowledge base  
> for future Bitcoin Core contributors, especially Chinese developers.

---

本仓库是我进入 **Bitcoin Core 开发** 过程中的系统阅读与思考笔记。

它不是官方指南，而是一个带有我个人判断的集合，包含：

- 与 Bitcoin Core 入门相关的 **原文文章、演讲与资源**  
- 我整理的 **高质量中文翻译**  
- 我作为开发者写下的 **技术批注与反思**  
- 从每篇文章中提炼出来的 **学习路径与资源地图**

目标是：

> 为未来想进入 Bitcoin Core 的开发者  
> ——特别是中文世界的开发者——  
> 提供一套可复用的高信噪比知识库。

---

## 2. Repository structure / 仓库结构

Current structure:

```text
bitcoin-core-onboarding/
├── README.md
└── 01-onboarding-to-bitcoin-core/
    ├── original.md               # Original article info & citation
    ├── faithful-translation.md   # 忠实中译
    ├── commentary.md             # 我的批注 & 延伸理解
    └── learning-map.md           # 从本文中提炼的学习资源地图

随着阅读与翻译的积累，我会继续添加新的目录，例如：
02-xxxx/
03-xxxx/
...
当文章和批注足够多时，会再整体重构为一个
全局学习地图（如 resources/global-learning-map.md），帮助读者按主题而不是按原文顺序学习。

3. Licensing & attribution / 版权与引用说明
	•	All original articles, blog posts and talks referenced here
remain under their original authors’ copyrights.
This repo only stores:
	•	Metadata (title, author, link), and
	•	My own translation and commentary as transformative work.
	•	If you are an original author and would like me to update or remove
something, please open an issue or contact me.

⸻

	•	本仓库所引用的原文文章、博客与演讲，版权均归原作者所有。
仓库中保存的是：
	•	原文的标题、作者与链接信息；
	•	以及我基于原文撰写的翻译与批注（属于二次创作）。
	•	如果你是原作者，并对本仓库中的整理方式有意见，欢迎通过 issue 或邮件与我联系，我会及时调整。

⸻

4. How to use this repo / 如何使用本仓库

For developers:
	•	Browse the folders by number (01-, 02-, …).
	•	Start with:
	•	faithful-translation.md if you prefer reading in Chinese;
	•	original.md if you want to follow the original English;
	•	commentary.md if you want my distilled takeaways;
	•	learning-map.md if you mainly want the resource graph.

For Chinese readers:
	•	可以按编号顺序阅读每一篇：
	•	想先了解原始语境：从 original.md 开始；
	•	想直接看中文：读 faithful-translation.md；
	•	想看「干货总结与开发者视角」：读 commentary.md；
	•	想快速找到所有提到的资料与链接：看 learning-map.md。

⸻

5. My personal context / 作者背景（简要）

I am working on Bitcoin script & Taproot engineering,
and writing an in-depth book tentatively titled

“Mastering Taproot”

This onboarding-notes repo is a parallel project:
it documents how I myself enter the Bitcoin Core codebase and culture,
in the hope that others can reuse the same path with less friction.

⸻

我目前专注于 Bitcoin Script 与 Taproot 工程实践，
并在撰写一本面向开发者的技术书籍（暂定名为《Mastering Taproot》）。

本仓库是一个与之并行的长期项目：
记录我自己如何进入 Bitcoin Core 代码库与社区文化，
也希望未来的开发者可以在这条路径上少走弯路。