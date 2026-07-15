---
title: "Auditoria LGPD"
nav_order: 7
parent: "Módulos"
permalink: /modulos/auditoria-lgpd/
task: modulo-lgpd
role: admin
routes: ["#/wp-admin/admin.php?page=rit360-solidario-lgpd"]
screenshots: [auditoria-lgpd]
source_docs: [solidario-privacy-ropa.md]
last_verified: 2026-07-15
status: publicado
---

# Auditoria LGPD

O RIT360 Solidário foi desenhado com a LGPD em mente. A tela **Auditoria LGPD**
reúne a trilha de ações sobre dados pessoais e um resumo das bases legais do
tratamento.

![Auditoria LGPD](/assets/img/auditoria-lgpd.png)

## O que a tela mostra

- Um **aviso com o resumo do tratamento** de dados e um link para a página de
  **Privacidade e bases legais** (o ROPA — registro de operações de tratamento).
- Uma **tabela somente leitura** com os últimos eventos: data, doador, ação, IP e
  o conteúdo (payload) de cada registro.

> 💡 **Nota — a OSC é a controladora**
>
> Quem responde pelos dados dos doadores é a **sua organização** (a controladora).
> A RIT/V3RTECH fornece o software. Esta tela ajuda você a demonstrar
> conformidade, mas as decisões e a responsabilidade sobre os dados são da OSC.

## Como o doador exerce os direitos dele

Um ponto importante: **a anonimização é feita pelo próprio doador**, no
[Portal do doador](/modulos/portal-do-doador/) — não pelo administrador. Lá o
doador pode revogar comunicações e **excluir/anonimizar os próprios dados**, com
dupla confirmação.

Ao anonimizar, os dados pessoais são substituídos por valores anônimos, mas os
**registros de doação são preservados** de forma anônima — porque a legislação
fiscal exige a guarda por alguns anos. O doador deixa de receber comunicações, e a
ação fica registrada nesta trilha de auditoria.

> ⚠️ **Atenção**
>
> Se um doador pedir a exclusão dos dados por e-mail, oriente-o a fazer isso pelo
> **portal do doador** (ele acessa por magic link, sem senha). É lá que a
> anonimização acontece, com a devida confirmação.

## Boas práticas de privacidade

> ✅ **Boas práticas**
>
> - Publique a **Política de Privacidade da sua OSC** e aponte para ela no
>   checkout (o consentimento do doador referencia essa política).
> - Exporte dados pessoais só quando necessário e prefira as versões
>   **mascaradas**.
> - Não compartilhe listas de doadores fora da organização.
