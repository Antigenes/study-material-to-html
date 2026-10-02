# Study Material to HTML

A Codex skill that turns user-provided slides, PDFs, documents, or notes into a complete, illustrated teaching HTML. It is designed for the learner who wants to study from the result without repeatedly reopening the source material.

这个 Codex skill 用于把课件、PDF、文档或笔记整理成可以独立学习的图解 HTML 教材。它强调讲清知识，而不是只把原文搬到网页里。

## What it guides Codex to do / 核心能力

- Inventory the source material and map substantive pages or sections to the lesson. / 逐页核对并建立内容覆盖关系。
- Explain concepts, algorithms, worked examples, proofs, complexity bounds, and edge cases. / 讲解概念、算法、例题、证明、复杂度与边界条件。
- Put original figures beside the explanations that use them, and explain animation frames step by step. / 保留原图，对动画分帧逐步讲解。
- Distinguish source claims, teaching additions, and corrections. / 区分课件原文、教学补充和需要指出的笔误。
- Build a readable offline HTML with navigation, useful interactions, and browser checks. / 生成适合学习的离线网页，并检查图片、交互和排版。

The skill adapts to the user's requested language, depth, audience, design, and output format. A single self-contained HTML is the default when practical.

## Install / 安装

Clone this repository into your Codex skills directory:

```bash
git clone https://github.com/Antigenes/study-material-to-html.git "${CODEX_HOME:-$HOME/.codex}/skills/study-material-to-html"
```

Then start a new Codex task and invoke `$study-material-to-html`, or ask Codex to make a comprehensive teaching HTML from your study materials.

之后开启新的 Codex 任务，附上学习材料并输入例如：

> 使用 `$study-material-to-html`，把这些课件做成中文教学 HTML。请完整覆盖内容，保留原图，逐步讲解算法和证明，让我只看网页就能学习。

## Repository layout / 仓库内容

```text
SKILL.md                  Skill entry point / skill 主说明
references/browser-qa.md  Browser and content QA checklist / 验收清单
LICENSE                   MIT License
```

This repository contains the reusable instructions only. Source decks and generated teaching pages are not included. / 仓库只包含可复用的 skill，不包含用户的课件或生成的教材。

## License

MIT. See [LICENSE](LICENSE).
