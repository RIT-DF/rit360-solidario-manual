---
title: "Blocos e Shortcodes"
nav_order: 11
parent: "Módulos"
permalink: /modulos/blocos-shortcodes/
task: modulo-shortcodes
role: admin
routes: []
screenshots: []
source_docs: [PRODUCT.md]
last_verified: 2026-07-15
status: publicado
---

# Blocos e Shortcodes

Shortcodes são pequenos códigos que você cola em qualquer página, post ou bloco do
seu construtor para inserir componentes do RIT360 Solidário. É assim que você monta
o hotsite de uma campanha com as peças do plugin.

## Shortcodes disponíveis

### `[rit360sol_doar]`
Exibe o formulário de doação de um projeto (valores, valor livre, frase de
impacto, vídeo, descrição e o botão **Doar agora**).

- Atributo: `id` — o ID do produto de doação. Sem ele, usa o projeto padrão.
- Exemplo: `[rit360sol_doar id="67"]`

### `[rit360sol_painel_doador]`
Exibe o **portal do doador** (a tela de acesso por magic link e, depois de logado,
as cinco abas). É o que fica na página `/minhas-doacoes`.

### `[rit360sol_projetos]`
Lista os seus **projetos** em cartões, lista ou grade.

- Atributos: `view` (`card` \| `list` \| `grid`), `ids`, `columns`, `limit`,
  `orderby`, `show_goal`.

### `[rit360sol_campanhas]`
Lista as suas **campanhas**, com progresso de meta.

- Atributos: `view`, `ids`, `columns`, `limit`, `orderby`, `show_goal`.

### `[rit360sol_transparencia]`
Página de **transparência pública**: mostra o arrecadado e o progresso das metas,
**sem expor nomes de doadores**. O resultado é armazenado em cache para não pesar
no site.

- Atributos: `view`, `scope` (`campanhas` \| `projetos`), `limit`, `columns`,
  `orderby`, `show_goal`.

> 💡 **Nota — compatibilidade**
>
> Os shortcodes `[rit360sol_doar]` e `[rit360sol_painel_doador]` também respondem
> pelos nomes antigos `[bs_doar]` e `[bs_painel_doador]`. Se você tinha páginas
> publicadas antes da mudança de marca, elas continuam funcionando.

> ✅ **Boas práticas**
>
> - Para o hotsite de uma campanha: combine `[rit360sol_transparencia]` (para
>   mostrar o progresso) com `[rit360sol_doar]` (para converter) na mesma página.
> - Os shortcodes funcionam em qualquer construtor (blocos do WordPress, Elementor,
>   etc.), porque são independentes do endereço da página.
