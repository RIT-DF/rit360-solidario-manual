# Roteiro de capturas — Manual RIT360 Solidário (v2.6.1)

Ambiente: **dev-wp** (`http://localhost:3080/`), plugin 2.6.1, OSC de exemplo
"Instituto Esperança", dados fictícios semeados. Viewport **1920×1080** em todas.
Destino dos arquivos: `manual/assets/img/`.

## Regras
- **Admin** (área `/wp-admin/`): capturar **logado** (a barra do WordPress pode
  aparecer — é a área administrativa).
- **Front-end** (`/doe`, transparência, portal do doador, checkout): capturar
  **deslogado do wp-admin** (um doador real NÃO vê a barra preta do WordPress).
  Usar contexto limpo / cookies zerados.
- Esperar a tela carregar antes de capturar. Preferir viewport (não fullPage),
  exceto onde indicado "página inteira".

## Admin — logado

| Arquivo | Rota | Deve mostrar |
|---|---|---|
| `painel.png` | `/wp-admin/admin.php?page=rit360-solidario` | KPIs + Top 10 doadores |
| `doadores-lista.png` | `…?page=rit360-solidario-donors` | Busca, tabela de doadores, ações em lote, blocos de exportação (página inteira) |
| `doador-detalhe.png` | clicar num doador da lista (ex.: Roberto Nascimento) | Dados + Recibos + Declarações |
| `projetos.png` | `…?page=rit360-solidario-projetos` | Lista de projetos com meta/campanha/padrão + form "Novo projeto" (página inteira) |
| `campanhas.png` | `…?page=rit360-solidario-campanhas` | Lista de campanhas com progresso vs meta |
| `prestacao-contas.png` | `…?page=rit360-solidario-prestacao-contas` | Filtro de período + totais + quebra por campanha/projeto + evolução (página inteira) |
| `config-organizacao.png` | `…?page=rit360-solidario-settings&tab=organizacao` | Formulário de dados da OSC |
| `config-visual.png` | `…&tab=visual` | Cores + preview |
| `config-lembretes.png` | `…&tab=lembretes` | Ativar lembretes + intervalo + envio manual |
| `config-emails.png` | `…&tab=emails` | Templates (assunto+corpo TinyMCE) + botão único "Salvar todos os templates" (página inteira) |
| `config-pdf.png` | `…&tab=pdf` | Cabeçalho/rodapé/recibo/declaração + pré-visualizar (página inteira) |
| `config-avancado.png` | `…&tab=avancado` | Reset de rate limit do magic link |
| `auditoria-lgpd.png` | `…?page=rit360-solidario-lgpd` | Aviso ROPA + tabela de auditoria |
| `shortcodes-tela.png` | `…?page=rit360-solidario-shortcodes` | Referência dos shortcodes em cards (tag + exemplo copiável + parâmetros), página inteira — v2.7.0 |
| `setup-wizard.png` | `…?page=bs-setup` | Passo 1 do Setup Wizard (Organização) |
| `produto-doacao.png` | editar produto 67 (`/wp-admin/post.php?post=67&action=edit`), aba "Configuração de Doação" | Campos: valores, valor livre, frase de impacto, vídeo |
| `feedback-modal.png` | qualquer tela do plugin → clicar "Enviar feedback" | Modal de feedback |

## Front-end — deslogado (sem barra do WordPress)

| Arquivo | Rota / ação | Deve mostrar |
|---|---|---|
| `doe-pagina.png` | `http://localhost:3080/doe/` | Imagem/título/frase de impacto + valores + "Doar agora" + vídeo + descrição (página inteira) |
| `checkout-doacao.png` | em `/doe`, escolher R$ 50 → "Doar agora" → checkout | Rótulos "Doar agora"/"Valor da doação", campo CPF, consentimento LGPD, "doar anonimamente" |
| `transparencia.png` | `http://localhost:3080/transparencia-teste/` | Cards de campanhas/projetos com arrecadado + barra de meta (sem nomes de doadores) |
| `portal-login.png` | `http://localhost:3080/minhas-doacoes/` | Formulário "Acessar meu painel" (e-mail + "Receber link") |
| `portal-doacoes.png` | portal logado (magic link donor 11) → aba "Minhas doações" | Histórico + "Baixar PDF" |
| `portal-dados.png` | aba "Meus dados" | Formulário editável (e-mail/CPF bloqueados) + zona de perigo |
| `portal-declaracao.png` | aba "Declaração anual" | Exercício + "Baixar declaração" |
| `portal-preferencias.png` | aba "Preferências" | Opt-in de lembretes |
| `portal-consentimentos.png` | aba "Consentimentos" | Consentimento c/ data + revogar + histórico |

### Magic link do portal (uso único — gerar fresco no contexto limpo)
```bash
docker exec dev-wp wp --allow-root eval '
global $wpdb; $b=random_bytes(32);
$plain=rtrim(strtr(base64_encode($b),"+/","-_"),"=");
$wpdb->insert($wpdb->prefix."bs_magic_links",[
 "donor_id"=>11,"token_hash"=>hash("sha256",$plain),
 "created_at"=>current_time("mysql"),
 "expires_at"=>date("Y-m-d H:i:s",time()+86400),
 "ip_address"=>"127.0.0.1","user_agent"=>"capture"]);
echo "http://localhost:3080/minhas-doacoes/?rit360sol_token=".$plain."\n";'
```
Navegar a URL retornada UMA vez; a sessão do doador fica ativa por cookie para as 5 abas.
