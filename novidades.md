---
title: "Novidades"
nav_order: 6
permalink: /novidades/
task: novidades
role: admin
source_docs: [CHANGELOG.md]
last_verified: 2026-07-15
status: publicado
---

# Novidades

O que mudou no RIT360 Solidário, em linguagem de quem usa. A versão instalada
aparece em **Plugins**, na lista de plugins do WordPress.

> 💡 **Nota**
>
> Esta é a versão amigável do histórico. O registro técnico completo fica no
> `CHANGELOG.md` do projeto.

---

## Versão 2.7 — Novos componentes para montar suas páginas

- **Botão de doação** (`[rit360sol_botao_doar]`): um botão pronto, com a cor da sua marca, que leva
  direto para a página da causa. Ótimo para chamar à ação no meio de um texto.
- **Barra de progresso** (`[rit360sol_meta]`): mostre só a barrinha "arrecadado × meta" de uma
  campanha ou projeto, onde você quiser.
- **Contador** (`[rit360sol_contador]`): exiba um número que engaja — "já arrecadamos R$ X",
  "N doações" — do total ou de uma campanha/projeto específico.
- **Listas na ordem que você quer**: em projetos, campanhas e transparência, agora dá para **ordenar**
  (por título, valor arrecadado ou percentual da meta) e mostrar, por exemplo, os **3 mais
  arrecadados**.
- **Nova tela "Shortcodes"** no menu do plugin: uma referência com todos os componentes, seus
  parâmetros e um botão **Copiar** em cada exemplo. (A antiga "Manual do Usuário" saiu do painel — o
  manual completo agora fica aqui, on-line.)

> **Atenção** — se você montou alguma página com os nomes antigos `[bs_doar]` ou
> `[bs_painel_doador]`, troque-os por `[rit360sol_doar]` e `[rit360sol_painel_doador]`: os apelidos
> antigos foram descontinuados.

---

## Versão 2.6 — E-mails com a cara da sua organização e página de doação mais rica

- Os **e-mails automáticos** (agradecimento, magic link, lembrete) agora herdam as
  **cores da sua identidade visual** — a faixa e o botão saem na sua marca, com o
  texto sempre legível.
- Os **templates de e-mail** ganharam um **único botão “Salvar todos”**: edite
  quantos modelos quiser e grave tudo de uma vez.
- A **página de doação** ficou mais rica: além dos valores e do botão, ela mostra a
  **imagem**, a **frase de impacto**, um **vídeo** e a **descrição** da causa — na
  ordem que mais converte.

> **Correções** — a **logomarca** da organização voltou a salvar corretamente nas
> configurações, e o **preenchimento automático de endereço pelo CEP** foi
> restabelecido.

---

## Versão 2.5 — Prestação de contas por campanha e projeto

- Nova visão de **prestação de contas** com quebra por **campanha e projeto**,
  evolução mensal e exportação em **PDF, CSV e XLSX** (com dados pessoais
  mascarados por padrão).
- O **recibo** e a **declaração anual** passaram a **discriminar o projeto** de
  origem da doação — muito mais clareza para o doador e para o conselho.
- Suporte ao novo **CNPJ alfanumérico** da Receita Federal.

---

## Versão 2.4 — Campanhas e metas

- Chegaram as **campanhas**: agrupe projetos, defina **meta** e **prazo** e
  acompanhe o **progresso** automaticamente.
- Página de **transparência pública** com o shortcode `[rit360sol_transparencia]`,
  mostrando o quanto foi arrecadado sem expor nomes de doadores.

---

## Versão 2.3 — Vários projetos de doação

- Agora a OSC pode ter **vários projetos**, cada um com sua página, seus valores e
  sua meta — em vez de um único “caixa” de doações.

---

## Versão 2.2 — Doações atribuídas a projetos

- Cada doação passou a ser **atribuída a um projeto**, base para os relatórios por
  causa que vieram depois.

---

## Versão 2.1 — Privacidade, bases legais e a barra da família

- Nova página de **Privacidade e bases legais** (o registro de tratamento de dados
  — ROPA) e um resumo na tela de LGPD do plugin.
- **Barra da família RIT360** no topo das telas, com acesso ao manual e ao
  **Enviar feedback**.
- Diversas correções de estabilidade nos formulários do painel.

---

## Versão 2.0 — Nova marca: RIT360 Solidário

- O plugin antes conhecido como **Bússola Solidária** passou a se chamar **RIT360
  Solidário**, integrando a família de produtos RIT360. As páginas e configurações
  existentes continuaram funcionando.
