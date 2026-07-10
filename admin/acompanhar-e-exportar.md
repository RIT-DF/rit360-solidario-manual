---
title: Acompanhar doações e exportar
parent: Administrador(a) da OSC
nav_order: 2
# --- contrato de handoff (docs-keeper) ---
task: acompanhar-e-exportar
role: admin
routes:
  - /wp-admin/admin.php?page=rit360-solidario
  - /wp-admin/admin.php?page=rit360-solidario-doacoes
  - /wp-admin/admin.php?page=rit360-solidario-doadores
source_docs: [PRD#6.13-M12, PRD#6.14-M13, PRD#5.5]
screenshots: [admin-painel-01, admin-doacoes-02, admin-doador-03, admin-export-04]
last_verified: 2026-07-04
status: publicado
---

# Acompanhar doações e exportar

No dia a dia você usa o painel para ver quanto foi arrecadado, consultar doações
e doadores, reenviar um recibo e exportar dados para a prestação de contas do
conselho.

## Ver os indicadores no painel

No menu do WordPress, abra **RIT360 Solidário**. O painel mostra os KPIs do
período (com seletor de **mês**, **ano** ou **personalizado**): total arrecadado,
número de doações, doadores únicos, ticket médio, retenção mensal e os principais
doadores.

![Painel com os KPIs do período](../assets/admin-painel-01.png)

## Consultar e filtrar doações

1. Abra **RIT360 Solidário → Doações**.
2. Use os filtros (período, status, valor, doador, forma de pagamento, produto)
   para encontrar o que procura.
3. Clique em uma linha para **ver o detalhe** da doação.

![Lista de doações com filtros](../assets/admin-doacoes-02.png)

## Atender um pedido de segunda via

Quando um doador pede a segunda via do recibo:

1. Abra **RIT360 Solidário → Doadores** e busque pelo e-mail.
2. Abra a **ficha do doador** — você vê todas as doações, consentimentos e
   comunicações.
3. Clique em **Reenviar recibo** (ou **Reenviar magic link**, se ele quiser
   acessar o próprio painel).

![Ficha do doador com as ações disponíveis](../assets/admin-doador-03.png)

{: .note }
> Também dá para reenviar a **declaração anual** e, a pedido do doador,
> **anonimizar** os dados dele (veja a futura página do LGPD Center).

## Exportar para a prestação de contas

Na lista de **Doações** ou de **Doadores**, use **Exportar** para gerar
**PDF**, **CSV** ou **XLSX** respeitando os filtros aplicados. O XLSX preserva
CPF, CEP e telefone como texto (não vira número), pronto para anexar à ata do
conselho.

![Menu de exportação em PDF/CSV/XLSX](../assets/admin-export-04.png)

## Dicas

- Todo mês você recebe um **e-mail com o resumo** do mês anterior — um bom gatilho
  para exportar e enviar ao conselho.
- Precisa das declarações anuais de todos os doadores? Use o disparo em **lote**
  na área de Relatórios (declaração anual em zip protegido).
