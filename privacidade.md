---
title: Privacidade e bases legais (ROPA)
nav_order: 7
permalink: /privacidade
# --- contrato de handoff (docs-keeper) ---
task: privacidade
role: ambos
source_docs: [projeto#8, solidario-privacy-ropa.md]
last_verified: 2026-07-11
status: publicado
---

# Privacidade e bases legais (ROPA)

Esta página descreve **quais dados pessoais** o RIT360 Solidário trata, **para quê**, sob **qual base
legal** da LGPD, por **quanto tempo** e **com quem** são compartilhados. É o Registro das Operações de
Tratamento (ROPA) do plugin, oferecido como modelo para a sua organização adotar e ajustar.

{: .nota }
> **Quem é a controladora.** O RIT360 Solidário roda no servidor da própria organização (auto-hospedado):
> os dados dos doadores ficam com você. Por isso **a sua OSC é a controladora** dos dados — quem define as
> finalidades. A RIT/V3RTECH fornece o software e **não** acessa nem armazena os dados dos seus doadores.

## Bases legais utilizadas (LGPD Art. 7)

- **Obrigação legal/regulatória (Art. 7, II)** — emissão e guarda do **recibo fiscal** e da **declaração
  anual** (nome, CPF, valor).
- **Consentimento (Art. 7, I)** — cadastro do doador e do consentimento LGPD **no ato da doação** (exigido
  no checkout).
- **Legítimo interesse (Art. 7, IX)** — **segurança** do acesso ao portal do doador, **gestão e métricas**
  internas da organização e **comunicações de relacionamento** (lembrete mensal) com o doador existente,
  sempre com **descadastro (opt-out) de 1 clique**.

## O que é tratado, para quê e por quanto tempo

| Atividade | Dados | Finalidade | Base legal | Retenção |
|---|---|---|---|---|
| Cadastro na doação | nome, e-mail, CPF (opcional), endereço/telefone, consentimento | Identificar o doador e viabilizar recibo, portal e métricas | Consentimento | Vinculada à guarda fiscal (5 anos) |
| Recibo e declaração anual | nome, CPF, e-mail, valor | Comprovante fiscal da doação | Obrigação legal | **5 anos** (fiscal) |
| Acesso ao portal (magic link) | e-mail, IP, dispositivo | Entrar sem senha; segurança/anti-abuso | Legítimo interesse | Links expirados: 30 dias; sessão: 2 h |
| Correção/atualização de dados | nome, telefone, endereço, preferências | Exercício de direitos do titular | Exercício de direitos (Art. 18) | Enquanto o cadastro existir |
| Anonimização | dados originais (substituídos) | Apagamento preservando a obrigação fiscal | Art. 18 + obrigação legal | Cadastro anonimizado permanece |
| Doação anônima | — (dados do pedido apagados) | Contabilizar sem reter identidade | — (sem dado pessoal) | Registro sem PII |
| Lembrete / agradecimento | e-mail, nome, total | Relacionamento com o doador | Legítimo interesse (opt-out) | Enquanto não houver opt-out |
| Painel e métricas | nome (e-mail mascarado nas telas) | Gestão da organização | Legítimo interesse | Enquanto o cadastro existir |
| Exportação de doadores | nome, e-mail, CPF, endereço | Exportação administrativa | Legítimo interesse | Arquivo sob controle do admin |

## Direitos do doador e como exercer

O doador acessa o **portal do doador** (link mágico enviado por e-mail, em `/minhas-doacoes/`) para:
**ver e corrigir** seus dados, ver o **histórico de ações** sobre eles, **descadastrar-se** de comunicações
e **anonimizar** os próprios dados (com dupla confirmação). O consentimento é registrado com data e hora
no momento da doação.

## Com quem os dados são compartilhados

- **WooCommerce** e o **gateway de pagamento** que a sua organização usar (fluxo de checkout, no seu servidor).
- **Envio de e-mail** (conforme a configuração de e-mail do seu site) — recibo, link de acesso, lembrete.
- **Geração de recibo/planilha** — processada **localmente** no seu servidor, sem envio a terceiros.
- **Não há mural público de doadores**: o ranking interno é visível apenas no admin, com e-mail mascarado.

{: .importante }
> Este é um modelo. A sua organização deve revisá-lo com sua assessoria e refletir a sua realidade na
> política de privacidade oficial (base legal, prazos e canais de contato do encarregado/DPO).
