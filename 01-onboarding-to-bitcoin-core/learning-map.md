Learning Map Extracted from “Onboarding to Bitcoin Core”
By Aaron Zhang

⸻

0. Overview / 全局结构

本文将 Amiti 原文中的所有学习资料，按照一个新人进入 Bitcoin Core 的真实流程，重新组织为五条主路径：
	1.	Foundational Knowledge / 概念底座
	2.	Staying Updated / 技术脉冲源
	3.	Codebase Mastery / 代码库掌握路径
	4.	Tools & Environment / 必备工具链
	5.	Community & Participation / 社区参与渠道

每条路径中的资源都包含：
	•	原文出处
	•	链接
	•	我对资源用途与优先级的总结

⸻

1. Foundational Knowledge

目的：建立理解 Bitcoin Core 所需的基础模型

⸻

1.1 必读文献（高优先级）

Bitcoin Whitepaper（强制）

如果没读，停止一切，先读这个。

	•	Link: https://bitcoin.org/bitcoin.pdf

用途：构建 UTXO / PoW / 分布式共识的最小模型。

⸻

1.2 必读教材（可选其一，但推荐组合）

Mastering Bitcoin — Andreas Antonopoulos
	•	Link: https://github.com/bitcoinbook/bitcoinbook
用途：技术深度适中、覆盖全面、最适合作为总览型教材。

Programming Bitcoin — Jimmy Song
	•	Link: https://github.com/jimmysong/programmingbitcoin
用途：Python 从零实现比特币，比教材更偏工程实践。

Grokking Bitcoin — Kalle Rosenbaum
	•	Link: https://github.com/kallerosenbaum/grokkingbitcoin
用途：图示化极佳，非常适合理解比特币内部运行逻辑。

⸻

1.3 系统课程

Chaincode Labs Bitcoin Curriculum（顶级）
	•	Link: https://github.com/chaincodelabs/bitcoin-curriculum
用途：唯一专门为“成为协议开发者”设计的课程。
涵盖：共识、mempool、P2P、签名、Taproot、审计。

⸻

1.4 资源大合集（查漏补缺）

Jameson Lopp – Bitcoin Information
	•	Link: https://www.lopp.net/bitcoin-information.html
用途：全网最全面的比特币资源索引，可随时查询。

⸻

2. Staying Updated

目的：持续保持对生态最新技术方向的感知

⸻

2.1 Weekly Pulse（最重要资源）

Bitcoin Optech Newsletter（新人的生命线）
	•	Link: https://bitcoinops.org/
用途：跟进 mempool、policy、BIP、实现进度的最有效方式。
作者 Dave Harding：业内认可的“文字魔术师”。

⸻

2.2 Mailing List & Discussion

bitcoin-dev / bitcoin-core-dev mailing list

用途：协议层讨论、BIP、软分叉、未来路线。

⸻

2.3 PR Review Club（社区最高性价比学习方式）

Bitcoin Core PR Review Club
	•	Link: https://bitcoincore.reviews/
用途：
	•	看真实 PR 的拆解与背景
	•	理解架构视角与审查逻辑
	•	提高自己未来做 review 的能力

这是新人真正能“跟得上 Core”节奏的重要基地。

⸻

3. Codebase Mastery

目的：真正开始理解 Bitcoin Core 的结构、模块与工作方式

⸻

3.1 必读开发文档

Contributing to Bitcoin Core（必读）
	•	包括：Review 原则、PR 风格、提交哲学。

Developer Notes（标准规范）
	•	用途：打开 PR 前必须复习，避免犯基础错误。

Productivity Notes（工程效率宝典）

推荐先掌握前四项：
	•	ccache
	•	./configure
	•	make -j [num-cores]
	•	build targets

用途：节省人生。

⸻

3.2 代码导航视频（我认为是最关键的两个）

Fabian Jahr – Debugging Bitcoin Core
	•	Link: https://www.youtube.com/watch?v=6aPSCDAiqVI
用途：新人的调试入门视频，是“怎么看懂代码路径”的最佳资源。

James O’Beirne – Bitcoin Core Architecture Overview
	•	Link: https://www.youtube.com/watch?v=L_sI_tXmy2U
用途：最高质量的 Bitcoin Core 架构鸟瞰图。

⸻

3.3 常用开发参考

Bitcoin Developer Reference（RPC & P2P）
	•	Link: https://developer.bitcoin.org/reference/
用途：查看消息格式、RPC 参数、链上字段。

⸻

3.4 StackExchange（高级问题的隐藏宝库）

Bitcoin StackExchange – Protocol Questions
	•	不佳于 Google 搜索，要直接去网站查。

用途：
高质量讨论集中在：script、P2P、validation、fees、wallet internals。

⸻

4. Tools & Environment

目的：构建一个能高效进行 Core 开发的工具链

⸻

4.1 Hands-on C++ 工具

tmux + C++ playground strategy

用途：隔离实验，验证 C++ 概念（initializer list 等）。

Compiler Explorer（强烈推荐）
	•	Link: https://godbolt.org/
用途：比较不同写法的优化差异、汇编输出。

CppCon Videos – Back to Basics Track

用途：快速建立现代 C++ 心智模型。

⸻

4.2 Git & IRC

IRC clients（原文推荐）
	•	irccloud（简单、开箱即用）

用途：
	•	#bitcoin-core-dev
	•	#bitcoin-core-pr-reviews
	•	#git
	•	##C++-general

⸻

4.3 Flashcards

Anki

用途：
记忆协议细节（Script rules, consensus flags, P2P messages）。

⸻

5. Community & Participation

目的：真正走进 Bitcoin Core 生态，建立贡献者身份

⸻

5.1 Regular Meetings

#bitcoin-core-dev weekly IRC meeting

时间：每周四 19:00 UTC
用途：
理解 Core 当前焦点 & 阶段性工作。

⸻

5.2 Conferences（高信噪比）

Bitcoin Edge Dev++（老但极高质量）
	•	2017: https://www.youtube.com/playlist?list=PLlWSs86hGNb8QKRuRP3maUsVmZm8uVmIR
	•	2018: https://www.youtube.com/playlist?list=PLlWSs86hGNb8bUsTnDmZz2ZvMfHy9fS_t

用途：
主题包括：共识、脚本、UTXO、网络层、软分叉机制。

⸻

5.3 Chaincode Residency（核心贡献路径）

Chaincode Residency

用途：
世界上最系统化的 Bitcoin Core onboarding 项目。
竞争激烈，但做贡献越多，越容易入选。

⸻

6. Find Your First PR

（作者最核心建议之一）

Amiti 的方法：
	1.	Watch good-first-issue
	2.	Watch up-for-grabs（包含已关闭的）
	3.	grep 代码库中的 TODO
	4.	跟一个代码子域的 PR
	5.	提供 follow-up / test coverage PR

我的总结（Aaron）：

新人不需要“任务”，需要的是“找到一个足够小的切片”。

Bitcoin Core 的世界没有人给你分配任务。
你必须自己定义它。

7. Closing Note

Amiti 的文章不仅仅是一个“资源列表”。
它实际上展示了一种路径：

如何从零开始，走上 Bitcoin Core 的学习、贡献与成长路线。

本 learning-map.md 把她的资源系统化整理，未来所有文章也会按这种格式提炼。
当积累到一定量，我会在 /resources/global-learning-map.md 中统一整合所有文章的学习图谱。