<h1 align="center">Questions your coding agent can't answer alone</h1>

<p align="center"><em>Stele before the plan · Prism before the edit · Shale after it</em></p>

Your coding agent hands you a diff. It does not say whether the change breaks
something you decided, whether it reached every place it had to, or what the
agent did and checked. Three local, open-source tools answer one question each.

| Tool | The question | What it does |
|---|---|---|
| **[Stele](https://github.com/provasign/stele)** (preview) | Does this break what we decided? | Checks every requirement against every one approved before it, and hands the agent the approved requirements a request touches. A request that cannot keep one makes the agent stop and ask you. |
| **[Prism](https://github.com/provasign/prism)** | Did it change everything it had to? | Every caller, override, implementation and test a change affects, resolved by the language's own compiler, not grep. Prism answers; the agent edits. |
| **[Shale](https://github.com/provasign/shale)** | What did the agent actually do? | Records the agent session (intent, files touched, checks run) and renders it as a card reviewers read before the diff. Gaps are shown, never hidden. |

Each tool stands alone. [Grove](https://github.com/provasign/grove), the code
graph under Prism, is open source too.

## Install

```sh
brew install provasign/tap/stele   # then: cd your-repo && stele init
brew install provasign/tap/prism   # then: cd your-repo && prism init
brew install provasign/tap/shale   # then: cd your-repo && shale init
```

Everything runs on your machine: no account, no server. Docs, benchmarks and
demos are at **[provasign.dev](https://provasign.dev)**.
