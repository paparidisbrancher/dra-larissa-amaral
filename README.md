# Site — Dra. Larissa Amaral

Site estático (sem build): `index.html` (CSS e JS embutidos), `privacidade.html`, `favicon.svg` e `assets/`.
Para ver localmente, abra o `index.html` no navegador.

**Estado: prévia.** Está com `noindex` e campos marcados "a confirmar". Não publicar como versão final
antes de a doutora revisar textos, alegações e imagens.

## A confirmar com a doutora

- [ ] WhatsApp: o link usa `553598196989`, copiado do Linktree (8 dígitos depois do DDD, formato antigo). Testar no celular e no computador.
- [ ] Nome completo e CRO-MG (seção Sobre e rodapé).
- [ ] Formação.
- [ ] "Dez anos de atuação" (bio do Instagram) continua valendo?
- [ ] Endereço completo e horário (seção Consultório e FAQ). Link de mapa só depois disso.
- [ ] Formas de pagamento (FAQ).
- [ ] Outros tratamentos além de facetas em resina.
- [ ] Retrato original **sem texto** e em alta resolução. O atual é recorte do post "Por que me escolher?" (720 px), só provisório.
- [ ] Um segundo retrato para a seção Sobre (hoje é outro recorte da mesma foto do topo, e no celular a repetição fica evidente).
- [ ] Fotos reais do consultório (entram na seção `#consultorio`, que hoje só tem texto).
- [ ] Logo oficial. A assinatura "Dra. Larissa Amaral" no topo e no rodapé é **provisória**, não é logo.
- [ ] Domínio definitivo (hoje as metatags apontam para `paparidisbrancher.github.io/dra-larissa-amaral/`).

## Como trocar

| O quê | Onde |
|---|---|
| WhatsApp | Buscar e substituir `553598196989` em `index.html` e `privacidade.html` (formato `55` + DDD + número, só dígitos). A mensagem inicial vem logo depois, em `?text=`. |
| CRO, formação | `index.html`, bloco `<dl class="dados">` da seção `#sobre`. No rodapé há um comentário marcando onde incluir. |
| Endereço, horário | `index.html`, seção `#consultorio`; resposta "Onde fica o consultório?" no FAQ; `address` no JSON-LD do `<head>`. |
| Retratos | `assets/larissa-retrato.webp` (hero, 630×522) e `assets/larissa-sobre.webp` (Sobre, 418×522). Mantendo nome e proporção, nada mais muda; mudando, ajustar `width`/`height` da `<img>`. |
| Imagem de compartilhamento | `assets/og-larissa.jpg` (1200×630). |
| Cores e fontes | Variáveis no `:root` no início do `<style>` do `index.html`. Fontes: Newsreader (títulos) e Manrope (texto), Google Fonts, licença OFL. |
| Logo | Trocar o `<a class="marca">` do cabeçalho e do rodapé por uma `<img>`. |

## Ao publicar a versão final

1. Remover `<meta name="robots" content="noindex, nofollow">` do `index.html`.
2. Atualizar `og:url`, `og:image` e o JSON-LD com o domínio definitivo; acrescentar `telephone` e `streetAddress` ao JSON-LD só com dados confirmados.
3. Conferir os links de WhatsApp no celular.

## Fotos e vídeos do Instagram (02/11/2026)

Extraídos com a conta do Erick logada no navegador, em resolução máxima. Vídeos em `videos/<código do reel>.mp4` (720p, só baixam ao dar play) com capa `.webp`. Confirmar com o cliente a autorização das pessoas que aparecem.
