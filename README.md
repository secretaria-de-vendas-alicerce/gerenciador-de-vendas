# Wrapper — Gerenciador de Vendas (Alicerce)

Página que embute o web app do Apps Script num `<iframe credentialless>`, contornando o roteador
de conta `/u/N/` do Google (a falha "Não foi possível abrir o arquivo" em navegador com 2+ contas
Google logadas). **Este é o link que a equipe deve usar** — nunca a `/exec` direta.

- `index.html` — o wrapper (embute a `/exec` do deployment de produção (`@5` v2.2.0), `AKfycbwdeGjw…`).
- `.nojekyll` — desliga o Jekyll no GitHub Pages.

Esta pasta é o ESPELHO da fonte (Regra 30): o repositório do Pages é montado fora do Drive
(Regra 7) a partir destes arquivos. Molde: `gerenciador-cca/wrapper/`.

Repo: **`secretaria-de-vendas-alicerce/gerenciador-de-vendas`** (público; o wrapper só carrega a
`/exec`, e o app tem login próprio). URL da equipe:
**`https://secretaria-de-vendas-alicerce.github.io/gerenciador-de-vendas/`**

Se a `/exec` mudar de `deploymentId`, atualizar o `src` do iframe **e** o `href` do fallback.
Publicar versão nova no MESMO id (`clasp update-deployment <id>`) mantém este link.
