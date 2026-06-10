# Provasign

Open-source tools for AI coding agents.

Our primary project is **Shale**: agent PR evidence that captures what an AI
coding agent was asked to do, what it touched, and what checks ran, then renders
that evidence on the pull request.

## Active Projects

| Repo | Role | License |
|---|---|---|
| **[shale](https://github.com/provasign/shale)** | Primary product: agent PR evidence, intent capture, session evidence, and PR cards | Apache-2.0 |
| **[prism](https://github.com/provasign/prism)** | Secondary product: graph-ranked context delivery for AI coding agents | MIT |
| **[grove](https://github.com/provasign/grove)** | Code graph engine for direct graph/index use and embedded tools | MIT |

## Install Shale

```sh
brew tap provasign/shale
brew install shale
cd your-repo
shale init
```

If Homebrew asks you to trust the tap:

```sh
brew trust --formula provasign/shale/shale
brew install shale
```

## What Shale Adds

- Agent intent recorded before the diff becomes review burden.
- Session evidence and local check history committed with the code.
- Pull-request cards that show what was seen, what was not seen, and what needs
  reviewer attention.
- No account, no hosted service, no GitHub App, and no token paste.

## Project Positioning

Use **Shale** when you want every agent-authored PR to explain itself.

Use **Prism** when you want agents to retrieve graph-ranked code context instead
of manually chasing `rg` results.

Use **Grove** when you want the graph directly for another project or custom
automation.
