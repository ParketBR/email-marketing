# Parket · E-mail marketing

Disparo em HTML para **público final**, com objetivo de gerar orçamento.

| | |
|---|---|
| Peça | [`parket-orcamento.html`](parket-orcamento.html) |
| Assunto e checklist | [`assuntos.md`](assuntos.md) |
| Imagens | [`imagens/`](imagens/) — 536 KB usados + alternativas |

## Padrão técnico

600px, tabelas aninhadas, CSS inline, fundo escuro. Compatível com Gmail,
Outlook desktop e web, Apple Mail, Yahoo, Mailchimp, RD Station e Brevo.

Sem WebP e sem SVG — nenhum dos dois renderiza de forma confiável em e-mail,
e todo o acervo de imagem da Parket está em WebP. As imagens deste repositório
já foram convertidas para JPG e recortadas em proporção fixa.

DM Sans só é aplicada onde o cliente suporta `@import` (Apple Mail, iOS). Nos
demais cai para Helvetica/Arial, que é o fallback do próprio design system.
Cores e tipografia vêm do `tokens.css` dos sites da marca.

A grade de soluções fica em 2 colunas também no mobile, de propósito: em
coluna única o e-mail dobraria de altura, e rolagem derruba taxa de clique.

## Antes de disparar

- [ ] Conferir o depoimento no perfil do Google, palavra por palavra
- [x] ~~Hospedar `imagens/` e trocar os `src`~~ — servidas pelo Pages deste repo
- [ ] Trocar `*|UNSUB|*` pela tag de descadastro da ferramenta
- [ ] Confirmar o WhatsApp comercial da campanha
- [ ] Teste de entrega em um Gmail, um Outlook e um iPhone

As imagens são servidas por <https://parketbr.github.io/email-marketing/imagens/>,
então o HTML já pode ser colado direto na ferramenta de disparo.

## Trocar uma foto

As candidatas estão em `imagens/alternativas/`, nos originais. Recorte na
proporção da faixa (12:7) ou do hero (3:2) antes de usar — o e-mail depende
de proporção fixa para as linhas não desalinharem.
