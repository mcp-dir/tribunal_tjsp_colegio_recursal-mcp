# Instalação detalhada

Tribunal TJSP: Colégio Recursal e Turma de Uniformização é um servidor MCP remoto. Aponte seu cliente pra `https://api.mcp.ai/p_tribunal_tjsp_colegio_recursal`. Snippets rápidos: [INSTALL.md](../INSTALL.md).

| Cliente | URL | Auth |
|---|---|---|
| Claude Desktop | `https://api.mcp.ai/p_tribunal_tjsp_colegio_recursal` | OAuth 2.1 ou agent-auth |
| Cursor | `https://api.mcp.ai/p_tribunal_tjsp_colegio_recursal` | OAuth 2.1 ou agent-auth |
| VS Code (Copilot) | `https://api.mcp.ai/p_tribunal_tjsp_colegio_recursal` | OAuth 2.1 ou agent-auth |

A config JSON é a mesma em todos: só a URL, sem headers.

## Desinstalar

Remova o bloco `mcpServers.tribunal_tjsp_colegio_recursal` (ou `servers.tribunal_tjsp_colegio_recursal` no VS Code) do config do cliente e reinicie.
