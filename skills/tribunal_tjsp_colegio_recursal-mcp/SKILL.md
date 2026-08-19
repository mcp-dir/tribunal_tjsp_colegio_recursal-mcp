---
name: tribunal_tjsp_colegio_recursal-mcp
description: Skill da REST API do Tribunal TJSP: Colégio Recursal e Turma de Uniformização na MCP.AI: 1 endpoint em /api/tribunal_tjsp_colegio_recursal. Tribunal TJSP: Colégio Recursal e Turma de Uniformização, consulta em fonte oficial. Hospedado pela plataforma, sem credenciais da plataforma, pague por consulta com crédito pré-pago. Autentique com workspace API key (sk_live) gerada em app.mcp.ai/settings/api-keys. Use quando o usuário pedir algo coberto pelos endpoints.
---

# Tribunal TJSP: Colégio Recursal e Turma de Uniformização — REST API skill

Você tem acesso à **Tribunal TJSP: Colégio Recursal e Turma de Uniformização** REST API na MCP.AI.

> Tribunal TJSP: Colégio Recursal e Turma de Uniformização, consulta em fonte oficial. Hospedado pela plataforma, sem credenciais da plataforma, pague por consulta com crédito pré-pago.

## Base URL

```
https://api.mcp.ai/api/tribunal_tjsp_colegio_recursal
```

Todo endpoint é um **POST** na Base URL + o path abaixo. Os parâmetros vão no corpo JSON.

## Autenticação

Inclua em toda request:

```
Authorization: Bearer sk_live_...
Content-Type: application/json
```

> Gere sua chave em **https://app.mcp.ai/settings/api-keys** (workspace API key `sk_live_…`, não expira, revogável). Uma única chave serve pra todos os seus MCPs.

## Formato de resposta

```json
{ "ok": true, "tool": "<tool_id>", "result": <payload> }
```

## Exemplo cURL

```bash
curl -X POST https://api.mcp.ai/api/tribunal_tjsp_colegio_recursal/consultar \
  -H "Authorization: Bearer sk_live_..." \
  -H "Content-Type: application/json" \
  -d '{}'
```

## Reportar problemas

Se um endpoint retornar erro, vazio ou dado inesperado, reporte (não desista calado): **POST /api/tribunal_tjsp_colegio_recursal/report** com `{ "message": "...", "context"?: "...", "conversation"?: [...] }`. Isso notifica o time da MCP.AI.

## Endpoints (1)

#### `tribunal_tjsp_colegio_recursal_consultar`

Tribunal TJSP: Colégio Recursal e Turma de Uniformização, consulta em fonte oficial. _(POST /api/tribunal_tjsp_colegio_recursal/consultar)_

| Parâmetro | Tipo | Obrigatório | Descrição |
|---|---|---|---|
| `numero_processo` | string | Não | Parâmetro de consulta "numero_processo". |
| `nome_parte` | string | Não | Parâmetro de consulta "nome_parte". |
| `rg` | string | Não | Parâmetro de consulta "rg". |
| `cpf` | string | Não | Parâmetro de consulta "cpf". |
| `nome_advogado` | string | Não | Parâmetro de consulta "nome_advogado". |
| `oab` | string | Não | Parâmetro de consulta "oab". |
| `secao` | string | Não | Parâmetro de consulta "secao". |
| `pagina` | string | Não | Parâmetro de consulta "pagina". |

---

Este MCP também funciona via **conexão MCP** (Claude / Cursor) em `https://api.mcp.ai/p_tribunal_tjsp_colegio_recursal` — veja o [README](../../README.md). A skill acima é pra consumir a **REST API** direto (agente próprio / código).
