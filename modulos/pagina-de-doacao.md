---
title: "Página de doação"
nav_order: 8
parent: "Módulos"
permalink: /modulos/pagina-de-doacao/
task: modulo-pagina-doacao
role: doador
routes: ["#/doe"]
screenshots: [doe-pagina, checkout-doacao]
source_docs: [PRODUCT.md]
last_verified: 2026-07-15
status: publicado
---

# Página de doação

É a página pública onde o doador contribui — normalmente em `/doe`. Ela foi
desenhada para converter: o essencial primeiro, os detalhes depois.

![Página de doação](/assets/img/doe-pagina.png)

## O que o doador vê

- A **imagem** e o **título** do projeto;
- a **frase de impacto** (ex.: “R$ 50 garantem uma cesta básica…”);
- os **valores sugeridos** e a opção **“Outro valor”** (com mínimo e máximo);
- o botão **Doar agora**;
- e, abaixo, o **vídeo** e a **descrição completa** da causa.

Essa ordem — ação primeiro, contexto depois — é intencional: quem já decidiu doa
sem rolar a página; quem quer saber mais encontra o conteúdo logo em seguida.

## O checkout da doação

Ao clicar em **Doar agora**, o doador vai para o checkout — que é o do
WooCommerce, mas com a linguagem trocada quando o carrinho tem só doação:

![Checkout da doação](/assets/img/checkout-doacao.png)

- Botão **“Doar agora”**, **“Valor da doação”**, **“Total da doação”** no lugar dos
  termos de loja;
- **Nome e e-mail** obrigatórios;
- **CPF/CNPJ** opcional, com o aviso de que é necessário para o recibo fiscal;
- **consentimento LGPD** obrigatório (com link para a política da OSC);
- opção **“Quero doar anonimamente”** (quando o carrinho é só doação);
- o **endereço** fica opcional se a OSC opera apenas com doações digitais.

> 💡 **Nota**
>
> O plugin só troca a linguagem quando o carrinho contém **apenas** produtos de
> doação. Se a OSC também vende outros produtos no mesmo site, o checkout comum do
> WooCommerce continua funcionando normalmente para eles.

## Depois da doação

- O doador vê uma **página de agradecimento**;
- recebe um **e-mail de reconhecimento** na hora (mesmo se o pagamento for PIX ou
  boleto, ainda pendente);
- e, quando o pagamento é confirmado, recebe o **recibo em PDF** por e-mail.

> ✅ **Boas práticas**
>
> Divulgue o link `/doe` em todos os canais e coloque um botão “Doar” bem visível
> no menu do site. A melhor página de doação é a que as pessoas conseguem
> encontrar.
