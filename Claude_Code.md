---
title: "Claude Code"
author: "Aman Jindal"
description: "Study Notes"
---

## Tools in Claude Code:

| **Name** | **Purpose** |
|---|---|
| Agent | Launch a subagent to handle a task |
| Bash | Run a shell command |
| Edit | Edit a file |
| Glob | Find files based upon a pattern |
| Grep | Search the contents of a file |
| LS | List files and directories |
| MultiEdit | Make several edits at the same time |
| NotebookEdit | Write to a cell in a Jupyter notebook |
| NotebookRead | Read a cell |
| Read | Read a file |
| TodoRead | Read one of the created to-do's |
| TodoWrite | Update the list of to-do's |
| WebFetch | Fetch from a URL |
| WebSearch | Search the web |
| Write | Write to a file |

---

## Claude Code Basic workflow:

- Explore
- Plan
- Code
- Commit

---

## Skills vs MCP vs Plugins vs Sub-Agents vs Hooks

| | **Skills** | **MCP** | **Plugins** | **Sub-Agents** | **Hooks** |
|---|---|---|---|---|---|
| **What it is** | Markdown instruction file | Protocol connecting Claude to external services | Bundled package of Skills, MCP, and commands | Spawned AI worker instance | Event-triggered scripts that fire at specific lifecycle points |
| **One-line role** | Teaches Claude how to work | Gives Claude access to external tools | Ready-made toolkit combining multiple components | An independent AI co-worker | Intercepts and acts at defined moments in Claude's workflow |
| **Analogy** | Recipe card | Kitchen plumbing | Full stocked kitchen | A hired specialist | A motion sensor that triggers an action |
| **Thinks independently** | No | No | No | Yes | No |
| **Works in parallel** | No | No | No | Yes | No |
| **Triggered by** | Task relevance | Tool call from Claude | Task relevance | Claude orchestrator | Lifecycle events (before/after tool use, before response, etc.) |
| **Setup effort** | Low | Medium | Low | Low | Medium |
| **Works offline** | Yes | No | Depends | Depends | Yes |
| **Built by** | You or community | Anthropic, providers, community | Anthropic or third parties | Claude automatically | You |
| **Best for** | Repeatable workflows, style guides | GitHub, Slack, databases, live APIs | Pre-built domain toolkits | Large parallel tasks | Logging, validation, guardrails, automation triggers |


---


