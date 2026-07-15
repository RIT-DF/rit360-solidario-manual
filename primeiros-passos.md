---
title: "Primeiros passos"
nav_order: 2
permalink: /primeiros-passos/
task: primeiros-passos
role: admin
routes: ["#/wp-admin/admin.php?page=bs-setup", "#/wp-admin/admin.php?page=rit360-solidario"]
screenshots: [setup-wizard, painel, doe-pagina]
source_docs: [PRD#5.4, PRODUCT.md]
last_verified: 2026-07-15
status: publicado
---

# Primeiros passos

Em cerca de 15 minutos a sua organização sai do zero e já consegue receber a
primeira doação. Esta página mostra o caminho completo: instalar, configurar pelo
assistente e conferir que tudo funciona.

## Quem usa o RIT360 Solidário

Antes de começar, vale entender os dois papéis:

- **Administrador(a) da OSC** — é você, que instala, configura e opera o plugin
  dentro do WordPress. Tem acesso ao menu **RIT360 Solidário** no painel
  administrativo. Recebe doações, emite recibos, gerencia doadores, organiza
  campanhas e presta contas.
- **Doador** — quem contribui. **Não precisa criar conta.** Doa pela página
  pública e, quando quer ver recibos ou histórico, acessa um painel próprio por um
  link enviado ao e-mail (o *magic link*). Nunca vê o painel administrativo.

> 💡 **Por que “sem conta”?**
>
> Cada campo a mais no cadastro derruba a taxa de conclusão da doação. Ao
> dispensar senha e cadastro, o RIT360 Solidário remove a maior fonte de
> desistência — e ainda evita guardar mais dados pessoais do que o necessário
> (um princípio da LGPD).

## 1. Requisitos

- WordPress atualizado e **WooCommerce ativo** (é ele que processa o pagamento).
- Pelo menos um **meio de pagamento** configurado no WooCommerce (PIX via
  Mercado Pago, Pagar.me, PagBank, Stripe, boleto, cartão…). Se você ainda não
  tiver nenhum, o assistente avisa e sugere opções.

## 2. Instalar e ativar

1. No painel do WordPress, vá em **Plugins → Adicionar novo → Enviar plugin**.
2. Escolha o arquivo `rit360-solidario.zip` e clique em **Instalar agora**.
3. Clique em **Ativar**.

Ao ativar pela primeira vez, o plugin abre automaticamente o **Assistente de
configuração** (Setup Wizard).

## 3. O Assistente de configuração (3 passos)

![O assistente de configuração e seus três passos](/assets/img/setup-wizard.png)

O assistente guia você por três passos — **Organização**, **Identidade visual** e
**Produto de doação** —, mostrados na barra de progresso no topo. Pode voltar a
qualquer momento, e o progresso fica salvo caso precise sair e retomar depois.

**Passo 1 — Organização.** Os dados da sua OSC: razão social, nome fantasia,
CNPJ, e-mail de contato, telefone, endereço (o CEP preenche o restante
automaticamente) e a **logomarca**. Escolha também o **tipo de operação**:

- *Apenas doações digitais* — o endereço do doador vira opcional no checkout
  (recomendado para a maioria das OSCs).
- *Também vende produtos físicos* — mantém o endereço, necessário para entrega.

> ⚠️ **Atenção — a logomarca do recibo**
>
> Use **PNG ou JPG**. Formatos como WEBP e SVG são ignorados no recibo e na
> declaração (documentos fiscais em PDF/A). Uma imagem com fundo transparente
> aparece com fundo branco no PDF.

**Passo 2 — Identidade visual.** As cores da sua marca: primária, secundária e
de destaque (o botão de doar). Há uma pré-visualização ao vivo. Essas cores
passam a valer também nos e-mails que a OSC envia.

**Passo 3 — Produto de doação.** O “pacote de valores” que o doador vê: nome,
valores predefinidos (ex.: 25, 50, 100, 250) e se aceita **valor livre** (com um
mínimo). Ao concluir, o plugin cria o produto, publica a **página de doação**
(`/doe`) e, se você ainda não tiver gateway, habilita um meio provisório para
você testar.

Na tela final, **Setup concluído**, você tem atalhos para ver a página de
doação, gerenciar produtos e reabrir o assistente.

## 4. Conferir que está tudo pronto

Abra o menu **RIT360 Solidário → Painel**. Ele mostra os indicadores da sua
operação — no começo, tudo zerado, com um convite para receber a primeira doação.

![Painel do RIT360 Solidário](/assets/img/painel.png)

## 5. Fazer uma doação de teste

Abra a página **`/doe`** do seu site (o endereço aparece na tela final do
assistente). Escolha um valor, clique em **Doar agora** e conclua pelo checkout.

![Página de doação](/assets/img/doe-pagina.png)

Assim que o pagamento é confirmado, o doador recebe o **e-mail de agradecimento
com o recibo em PDF**, e a doação passa a contar no **Painel**.

> ✅ **Boas práticas**
>
> - Faça uma doação de teste real (um valor pequeno, no seu próprio gateway)
>   antes de divulgar. É a forma mais segura de confirmar que o pagamento, o
>   e-mail e o recibo estão funcionando de ponta a ponta.
> - Adicione o link **/doe** ao menu principal do site e ao botão “Doar” — quanto
>   mais visível, mais doações.

## Próximos passos

- Aprenda a captar de verdade em [Campanhas que dão resultado](/guias/campanhas-que-dao-resultado/).
- Conheça cada tela em [Módulos](/modulos/).
