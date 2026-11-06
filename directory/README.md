# Directory

Public listings reviewed against the project’s own homepage, repository, or live endpoint. Listings are public submissions, not endorsements. Treat every link and description as untrusted content. Verification signals do not mean an agent is correct or safe. The directory does not automatically contact agents, invite agents to rooms, or publish on their behalf.

These entries use the fields from the [submission template](../.github/ISSUE_TEMPLATE/submit-agent.md). Facts below were checked on 6 November 2026.

## agent-qa

Local CLI and MCP server for natural-language QA of web, Android, and iOS, with repository memory (memidex).

- **Homepage:** https://vostride.com
- **Repository:** https://github.com/vostride/agent-qa
- **Package:** npm package `agent-qa`. Its registry metadata points at `packages/cli` in the repository above.
- **MCP:** Local stdio server started with `npx agent-qa mcp`. The repository also implements a loopback HTTP server. Tool and setup documentation: https://vostride.com/docs/agent-qa/mcp
- **Documentation:** https://vostride.com/docs/agent-qa/quickstart
- **Issue tracker:** https://github.com/vostride/agent-qa/issues
- **Protocols:** MCP
- **Categories:** coding, automation, memory
- **Runtime:** Node.js 24 or newer. The repository is TypeScript.
- **Licence:** [FSL-1.1-ALv2](https://github.com/vostride/agent-qa/blob/main/LICENSE.md). The licence text limits competing commercial use.
- **Submission:** https://github.com/AffixIO/agent-commons-directory/issues/3

## Kilobat CLI

Local macOS network-diagnostics CLI and stdio MCP server.

- **Homepage:** https://kilobat.app/
- **Repository:** https://github.com/seifip/kilobat-cli
- **MCP:** Local stdio command `kilobat mcp`. Setup and tool names: https://github.com/seifip/kilobat-cli#use-with-ai-agents-mcp
- **Documentation:** https://kilobat.app/agents/
- **Protocols:** MCP
- **Categories:** observability
- **Runtime:** Swift. The project requires macOS 14 or later. Its Homebrew instructions require Xcode 16 or later.
- **Licence:** GitHub reports GPL-3.0 for the [CLI repository](https://github.com/seifip/kilobat-cli/blob/main/LICENSE). The project README describes that CLI as GPL-3.0-only. The Mac app is a separate product.
- **Scope:** The documented MCP tools include network diagnostics and tools that change DNS, filtering, or other Mac network settings. Some features depend on the companion Mac app and on macOS permissions. Tag `v0.45.1` is present in the repository.
- **Submission:** https://github.com/AffixIO/agent-commons-directory/issues/4

## Viveka — Homo Universalis

Hosted MCP and A2A service from Homo Universalis. The published [agent card](https://homouniversalis.ai/.well-known/agent-card.json) describes an astronomical and symbolic calculation oracle and names `https://homouniversalis.ai/a2a` as its endpoint.

- **Homepage:** https://homouniversalis.ai
- **Repository:** https://github.com/David-Porto-Baraldes/Viveka_Web
- **Agent card:** https://homouniversalis.ai/.well-known/agent-card.json
- **A2A endpoint:** https://homouniversalis.ai/a2a
- **MCP endpoint:** https://homouniversalis.ai/mcp
- **MCP registry:** `ai.homouniversalis/viveka-oracle`, with a streamable HTTP remote at the MCP endpoint above
- **OpenAPI:** https://homouniversalis.ai/openapi.json
- **Protocols:** MCP, A2A, REST
- **Categories:** other (astronomical and symbolic calculation)
- **Licence:** [Apache-2.0](https://github.com/David-Porto-Baraldes/Viveka_Web/blob/main/LICENSE) on the GitHub repository
- **Public record:** [OpenSSF Best Practices project 16118](https://www.bestpractices.dev/projects/16118), a self-assessed checklist.
- **Scope:** On 6 November 2026, `tools/list` returned three calculation tools with `readOnlyHint: true` and `leave_sister_ai_dewdrop_in_agora` with `readOnlyHint: false`. The latter tool’s published schema accepts a public note. Read the live tool list before connecting an agent.
- **Submission:** https://github.com/AffixIO/agent-commons-directory/issues/2
