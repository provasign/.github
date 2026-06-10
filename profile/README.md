<p align="center">
  <img src="https://raw.githubusercontent.com/provasign/shale/main/assets/brand/shale-icon.svg" alt="" width="72">
</p>

<h1 align="center">Open-source tools for AI coding agents</h1>

<p align="center"><em>Every agent PR should explain itself.</em></p>

Our primary project is **Shale**: agent PR evidence that captures what an AI
coding agent was asked to do, what it touched, and what checks ran — then
renders that evidence as a card on the pull request.

<p align="center">
  <img src="https://raw.githubusercontent.com/provasign/shale/main/assets/brand/shale-demo.svg" alt="A Shale session: shale intent, agent edits, shale done, git push, card rendered" width="720">
</p>

## Projects

| Repo | Role | License |
|---|---|---|
| **[shale](https://github.com/provasign/shale)** | Agent PR evidence: intent capture, session evidence, and PR cards — the primary project | Apache-2.0 |
| **[prism](https://github.com/provasign/prism)** | Graph-ranked context delivery for AI coding agents (CLI + MCP) | MIT |
| **[grove](https://github.com/provasign/grove)** | Persistent code-graph engine: Tree-sitter parsing, SQLite, impact and test queries | MIT |
| **[fuse](https://github.com/provasign/fuse)** | Symbol-aware Git merge driver built on Grove | MIT |

## Try Shale in five minutes

```sh
brew install provasign/shale/shale
cd your-repo
shale init
git add . && git commit -m "chore: enable shale" && git push
```

No account, no server, no GitHub App, no token paste. The next agent-authored
PR carries a card — see the
**[live demo pull requests](https://github.com/provasign/shale-test-bed/pulls?q=is%3Apr)**
for real examples, or start with the
**[getting-started guide](https://github.com/provasign/shale/blob/main/docs/getting-started.md)**.

## Which tool do I want?

- **Shale** — you want every agent-authored PR to explain itself to reviewers.
- **Prism** — you want agents to retrieve graph-ranked code context instead of
  chasing `rg` results across a dozen file reads.
- **Grove** — you want the code graph itself: indexing, symbols, blast radius,
  test coverage queries, embeddable Go API.

Everything is local-first and fail-open by design. Docs live at
**[provasign.dev](https://provasign.dev)**.
