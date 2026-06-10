# Provasign

Open-source tools for AI coding agents.

The public focus of this org is now **Shale**: agent PR evidence that captures
what an AI coding agent was asked to do, what it touched, and what checks ran,
then renders that evidence on the pull request.

The hosted/enterprise Provasign product is paused and intentionally hidden for
now. We are keeping the org name because the repositories, packages, releases,
and Homebrew taps already live here.

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

Provasign as a certification product may return later, but it is not the
current public product path.
