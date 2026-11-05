<p align="center">
  <img src="assets/plain-ayi-icon.png" alt="Plain-AyI" width="96" height="96">
</p>

<h1 align="center">Plain-AyI</h1>

<p align="center">
  <b>Open-source AI projects, explained in plain words.</b><br>
  A free, read-only guide for non-technical people and developers, with a connector for AI assistants.
</p>

<p align="center">
  <a href="https://plain-ayi.com">plain-ayi.com</a> ·
  <a href="https://plain-ayi.com/new">New this week</a> ·
  <a href="https://plain-ayi.com/connect">Connector setup</a> ·
  <a href="https://plain-ayi.com/privacy">Privacy</a>
</p>

<p align="center">
  <a href="https://mcptry.com/servers/io.github.AyodejiOO/plain-ayi"><img src="https://mcptry.com/badge/io.github.AyodejiOO/plain-ayi" alt="mcptry status"></a>
</p>

---

## What it is

Some of the most useful AI tools are open source, but they're scattered across GitHub and described in developer language. [Plain-AyI](https://plain-ayi.com) gathers a growing, non-exhaustive list of them and explains each one in everyday words:

- what it does and who it's for
- whether you need to code
- what it costs, including when a paid AI account is needed
- whether your data stays on your device
- simple first steps, with safety notes before you install anything

New projects are added every day. Ratings reflect public activity (stars, contributors, downloads, recent updates), not a verdict on which project matters most.

## Use it from your AI assistant

Plain-AyI has a read-only MCP connector, so your AI assistant can search the guide for you, for example *"find me a free tool that turns my voice recordings into text, without them leaving my laptop"*.

**Connector address:** `https://plain-ayi.com/mcp`. No account or API key is needed.

<details open>
<summary><b>Claude (web, desktop and mobile)</b></summary>

Find **Plain-AyI** in Claude's connector directory and click **Connect**. Or add it yourself: **Customize → Connectors → Add custom connector**, name it `Plain-AyI`, and paste `https://plain-ayi.com/mcp`.
</details>

<details>
<summary><b>Claude Code</b></summary>

```bash
claude mcp add --transport http plain-ayi https://plain-ayi.com/mcp
```
</details>

<details>
<summary><b>Cursor</b></summary>

Add to `~/.cursor/mcp.json`, or to `.cursor/mcp.json` in a project:

```json
{
  "mcpServers": {
    "plain-ayi": { "url": "https://plain-ayi.com/mcp" }
  }
}
```
</details>

<details>
<summary><b>GitHub Copilot in VS Code</b></summary>

Add to `.vscode/mcp.json` in your project:

```json
{
  "servers": {
    "plain-ayi": { "type": "http", "url": "https://plain-ayi.com/mcp" }
  }
}
```
</details>

<details>
<summary><b>Gemini CLI</b></summary>

Install it as an extension:

```bash
gemini extensions install https://github.com/AyodejiOO/plain-ayi-connector
```

Or add to `~/.gemini/settings.json`:

```json
{
  "mcpServers": {
    "plain-ayi": { "httpUrl": "https://plain-ayi.com/mcp" }
  }
}
```
</details>

### Tools

| Tool | What it does |
|---|---|
| `search_projects` | Finds projects by what they do, with optional category and "no coding needed" filters |
| `get_project` | Full details of one project: cost, privacy, licence, first steps and official links |
| `list_categories` | The categories in the guide |

All three tools are read-only. The connector can't change anything, and it keeps no record of who asked. See the [privacy page](https://plain-ayi.com/privacy).

Also listed in the [official MCP Registry](https://registry.modelcontextprotocol.io/) as `io.github.AyodejiOO/plain-ayi`.

## Feedback

Spotted a wrong description, or looking for a tool that isn't listed? [Open an issue](https://github.com/AyodejiOO/plain-ayi-connector/issues), or use the "Report a problem" link on any project page.

## About

Plain-AyI is an independent, non-commercial project by [Ayodeji Ogunniyi](https://x.com/ayodeji_FG), made as a small way of giving back to the open-source community. With gratitude to everyone who builds in the open and makes intelligence more accessible at no cost.

Plain-AyI links to each project's official pages but doesn't host, review or endorse their software. Please download and install at your own discretion.

This repository holds the connector's public description and setup files. The website's source is maintained separately.
