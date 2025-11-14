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
- 从每篇文章中提炼的 **学习路径与资源地图**

目标是：

> 为未来想进入 Bitcoin Core 的开发者  
> ——特别是中文世界的开发者——  
> 提供一套可复用的高信噪比知识库。

---

## 2. Repository structure / 仓库结构

Current structure:

```
bitcoin-core-onboarding/
├── README.md
└── 01-onboarding-to-bitcoin-core/
    ├── original.md
    ├── faithful-translation.md
    ├── commentary.md
    └── learning-map.md
```

随着阅读与翻译的积累，我会继续添加新的目录，例如：

```
02-xxxx/
03-xxxx/
...
```
当文章与批注积累到一定规模，我会将其进一步整理为一个全局学习地图，例如：

```
resources/
└── global-learning-map.md
```

该文件将帮助读者按照主题（如脚本、共识、网络、测试框架、C++ 等）系统性学习，而不是按原文顺序阅读。

---

## 3. Licensing & attribution / 版权与引用说明

All original articles, blog posts, and talks referenced here remain under their original authors’ copyrights.  
This repo only stores:

- Metadata (title, author, link)  
- My own translation and commentary as transformative work

If you are an original author and would like me to update or remove something, please open an issue.

---

本仓库所引用的原文文章、博客与演讲，其版权均归原作者所有。  
本仓库仅保存：

- 原文的标题、作者与链接  
- 我基于原文撰写的翻译与批注（属于二次创作）

如原作者希望更新或移除内容，欢迎通过 issue 与我联系。

---

## 4. How to use this repo / 如何使用本仓库

For developers:

- Browse the folders in numerical order (01-, 02-, …)  
- Read:
  - `original.md` for the original English  
  - `faithful-translation.md` for high-fidelity Chinese  
  - `commentary.md` for distilled insights  
  - `learning-map.md` for all extracted resources

For Chinese readers:

- 按编号顺序阅读每篇内容  
- 想看英文原文：阅读 `original.md`  
- 想快速进入中文：阅读 `faithful-translation.md`  
- 想看我的精华总结：阅读 `commentary.md`  
- 想快速掌握所有资料链接：阅读 `learning-map.md`

---

## 5. My personal context / 作者背景（简要）

I currently focus on **Bitcoin programming, developer education,  
and engineering practices built on top of the Taproot upgrade**.  
I am also writing a developer-focused technical book titled:

**“Mastering Taproot”**

This repo documents my own onboarding path into Bitcoin Core.

---

我目前专注于 **Bitcoin 编程、开发者教育，以及基于 Taproot 升级的工程实践**，  
并在撰写一本面向开发者的技术书籍：

**《Mastering Taproot》**

本仓库记录了我进入 Bitcoin Core 代码库与社区文化的路径，  
也希望未来的开发者可以复用这条路线。