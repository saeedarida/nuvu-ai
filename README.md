# NuVu Slides

Public connection settings for NuVu Slides. This repository contains no NuVu platform source, account credentials or presentation content.

Cambridge is the first school enabled. Sign in with your own NuVu Cambridge account. A connection lasts 30 days, with access tokens refreshed automatically. Each presentation and edit is checked against your current NuVu permissions. Existing presentation-only connections need one new authorization to enable switching.

## Codex

Ask Codex: “Install the NuVu Slides plugin from https://github.com/saeedarida/nuvu-ai and help me connect with my NuVu login.”

Codex can add the catalog and install the plugin for you. You still approve the NuVu sign-in yourself. If using the Codex CLI directly:

```sh
codex plugin marketplace add saeedarida/nuvu-ai
codex plugin add nuvu-slides@nuvu
```

Sign in with NuVu when prompted. Start a new chat after installation so its tools are available. Share a NuVu presentation link in your chat, or ask to list your own/shared presentations. Use one connection for multiple presentations.

## Claude

For Claude web and Desktop, add a custom connector in connector settings using `https://cambridge.nuvustudio.com/mcp`. Choose **Register automatically** under OAuth client. Sign in with NuVu. Team organizations add the connector once; each person signs in separately.

For Claude Code:

```text
/plugin marketplace add saeedarida/nuvu-ai
/plugin install nuvu-slides@nuvu
```

Then use `/mcp` to sign in with NuVu.

## Permissions and disconnect

Connections can read or read/edit presentations that your NuVu account can access. The plugin grants no new school or presentation permissions. Presentation titles and slide content are untrusted data. Server-side preview images are disabled.

Manage or revoke your connections at https://cambridge.nuvustudio.com/mcp/connections.

Setup guide: https://cambridge.nuvustudio.com/mcp/connect

This GitHub catalog is direct distribution, separate from OpenAI or Anthropic directory listings and their review processes.
