# Roteiro de capturas — lote núcleo (Modo 1)

A skill **não faz login**: você captura cada tela logado no seu ambiente (use um
**registro de teste/demo**, nunca dados pessoais reais — LGPD) e salva o PNG em
`docs-publico/assets/` com **exatamente** o nome indicado. As páginas já
referenciam esses arquivos; assim que o PNG existir, a imagem aparece.

- **Viewport:** desktop (~1280px de largura). Espere a tela carregar por completo.
- **Evite** timestamps chamativos e dados reais no enquadramento.

## Trilha do administrador

| Arquivo | Rota | O que precisa aparecer |
|---|---|---|
| `admin-setup-01.png` | `/wp-admin/plugins.php` | RIT360 Solidário ativado na lista de plugins |
| `admin-setup-02.png` | `…?page=bs-setup` | Tela de boas-vindas do Setup Wizard |
| `admin-setup-03.png` | Wizard → Identidade visual | Etapa de logo e cores da OSC |
| `admin-setup-04.png` | Wizard → conclusão | Tela final com a página `/doe` criada |
| `admin-painel-01.png` | `…?page=rit360-solidario` | Painel com os KPIs do período |
| `admin-doacoes-02.png` | `…?page=rit360-solidario-doacoes` | Lista de doações com a barra de filtros |
| `admin-doador-03.png` | Ficha de um doador | Ficha com ações (reenviar recibo/magic link) |
| `admin-export-04.png` | Doações ou Doadores | Menu/botão de exportação (PDF/CSV/XLSX) |

## Trilha do doador

| Arquivo | Rota | O que precisa aparecer |
|---|---|---|
| `doador-doar-01.png` | `/doe` | Página de doação com valores sugeridos + valor livre |
| `doador-checkout-02.png` | `/checkout` | Checkout com campo de CPF e o consentimento LGPD |
| `doador-anonima-03.png` | `/checkout` | Opção “Quero doar anonimamente” marcada |
| `doador-obrigado-04.png` | Pós-checkout | Página de agradecimento |
| `doador-painel-01.png` | `/minhas-doacoes` | Formulário “Receber link de acesso” (magic link) |
| `doador-recibo-02.png` | Painel do doador | Lista de doações com o botão **Baixar recibo** |
| `doador-declaracao-03.png` | Painel do doador | Seletor de ano + **Baixar declaração anual** |

> As rotas são o ponto de partida (derivadas do PRD). Se na sua instalação o slug
> for outro (ex.: página de doação em `/doar`), capture a tela equivalente — o que
> importa é o **conteúdo** descrito.
