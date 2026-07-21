---
title: "Portal do doador"
nav_order: 9
parent: "Módulos"
permalink: /modulos/portal-do-doador/
task: modulo-portal-doador
role: doador
routes: ["#/minhas-doacoes"]
screenshots: [portal-login, portal-doacoes, portal-dados, portal-declaracao, portal-preferencias, portal-consentimentos]
source_docs: [PRODUCT.md]
last_verified: 2026-07-21
status: publicado
---

# Portal do doador

O portal é o espaço de autoatendimento do doador — normalmente em
`/minhas-doacoes`. Ele acessa **sem senha e sem conta**: informa o e-mail e recebe
um link de acesso (o *magic link*).

## Acesso por magic link

![Portal do doador — acesso](/assets/img/portal-login.png)

O doador digita o e-mail e clica em **Receber link de acesso**. Por segurança, a
mensagem na tela é sempre a mesma (não revela se o e-mail está ou não cadastrado),
e o link recebido **expira em 24 horas** e serve **uma única vez**.

> 💡 **Por que sem senha?**
>
> Senha é mais uma barreira — e mais um dado para guardar e vazar. O magic link
> dá acesso seguro sem nada disso: quem tem acesso ao e-mail do doador é o próprio
> doador.

## As cinco abas

**Minhas doações** — o histórico completo, com **download do recibo em PDF** de
cada doação.

![Portal — Minhas doações](/assets/img/portal-doacoes.png)

**Meus dados** — o doador edita nome, telefone e endereço. O **e-mail e o documento
não são editáveis** (são a identidade do registro): para pessoa física aparece o
**CPF** mascarado; para pessoa jurídica, a **razão social** e o **CNPJ** mascarado.
Aqui também fica a “zona de perigo” para **excluir os próprios dados**.

![Portal — Meus dados](/assets/img/portal-dados.png)

**Declaração anual** — o doador escolhe o exercício (ano) e baixa a **declaração
consolidada**, útil na época do Imposto de Renda.

![Portal — Declaração anual](/assets/img/portal-declaracao.png)

**Preferências** — liga ou desliga o **lembrete mensal** de doação.

![Portal — Preferências](/assets/img/portal-preferencias.png)

**Consentimentos** — mostra o consentimento LGPD (com data e hora), permite
**revogar comunicações** e traz o histórico de ações. É também por aqui que o
doador pode **anonimizar os próprios dados**, com dupla confirmação.

![Portal — Consentimentos](/assets/img/portal-consentimentos.png)

> ⚠️ **Atenção**
>
> A exclusão/anonimização é definitiva: os dados pessoais são substituídos por
> valores anônimos. Os **registros de doação são preservados** de forma anônima
> (exigência fiscal), mas o doador deixa de receber comunicações e não é mais
> identificável.

> ✅ **Boas práticas**
>
> Adicione o link **“Minhas doações”** ao rodapé do site. Assim, quem precisa de
> uma segunda via de recibo se resolve sozinho — e a sua OSC recebe menos pedidos
> de suporte.
