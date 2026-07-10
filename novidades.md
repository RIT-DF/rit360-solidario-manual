---
title: Novidades
nav_order: 8
# --- contrato de handoff (docs-keeper) ---
task: novidades
role: ambos
source_docs: [CHANGELOG.md]
last_verified: 2026-07-04
status: publicado
---

# O que há de novo

Resumo, em linguagem leve, das novidades mais recentes. Para o histórico técnico
completo, veja o `CHANGELOG.md` do projeto.

## Versão 1.4.4
- **Checkout mais robusto:** corrigido um problema em que o campo de consentimento
  podia bloquear a finalização de compras que **não eram doações** no checkout em
  blocos. Doações seguem exigindo o consentimento normalmente.

## Versão 1.4.3
- **Campos de doação também no checkout clássico:** o plugin agora detecta quando a
  página de checkout não usa blocos e ajuda a converter em um clique.
- **Reconhecimento imediato no PIX:** ao doar por PIX/boleto, você recebe um e-mail
  de “recebemos sua doação” da organização, além do e-mail com o QR Code.

## Versão 1.4.x — Recibos e declarações no seu jeito
- **Personalização do recibo e da declaração:** cabeçalho e rodapé, texto jurídico
  e mensagem extra passam a ser editáveis, com pré-visualização.

## Versão 1.3.0 — Trabalho em lote
- **Ações em lote na lista de doadores:** enviar lembrete, exportar selecionados e
  gerar a declaração anual de vários doadores em um único arquivo `.zip`.
- **Exportar doadores em XLSX:** planilha completa, com CPF/CEP/telefone como texto.

{: .note }
> Está usando uma versão anterior? Confira em **Bússola Solidária → Sobre** e peça
> a atualização à equipe que cuida do seu site.
