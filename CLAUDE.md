# Headtuff: contexto do projeto

Marca brasileira de bonés street. Este repositório é o site **headtuff.com**. Responda sempre em português do Brasil.

## Marca
- **Nome:** Headtuff ("tuff" é gíria de "brabo, estiloso"). Instagram e TikTok: **@useheadtuff**. Domínio: **headtuff.com** (comprado na Hostinger).
- **Público:** 16 a 24 anos, estética street. Preços de R$100 a R$180.
- **Frase de assinatura:** "Cabeça dura desde sempre."
- **Conceito da coleção:** "Não precisa gritar o nome. Quem é da rua reconhece."
- **Logo principal:** "Headtuff" em letra cursiva fina. No site usamos a fonte Pinyon Script como provisória; o logo final deve ser desenhado.
- **Referência de site e branding:** wantsandneeds.com (estrutura da loja). Nunca copiar textos, fotos ou logos de lá.

## Drop 001: Coleção Sombra (lote de 300)
Todos os bonés seguem as mesmas regras: logo cursivo tom sobre tom na frente, corda trançada entre a copa e a aba, "001" bordado na lateral esquerda, faixa interna com "Cabeça dura desde sempre" e regulagem traseira com fivela.

| Boné | Visual | Qtd. | Preço |
|---|---|---|---|
| Sombra Preto | Preto, logo grafite, corda branca | 90 | R$129 |
| Sombra Osso | Osso, logo areia, corda preta | 50 | R$129 |
| Sombra Marinho | Marinho, logo azul aço, corda creme e marinho | 40 | R$139 |
| Sombra Garrafa | Verde garrafa, logo musgo, corda creme e verde | 40 | R$139 |
| Sombra Lavado | Preto estonado, logo cinza desbotado, aba desfiada | 30 | R$149 |
| Sombra Flash | Preto, cursiva gigante em linha refletiva, 50 numerados | 50 | R$179 |

**Oferta:** leve 2 por R$239 (o Flash não entra), Pix com 5% de desconto ou 3x sem juros, frete grátis acima de R$250 e troca em 30 dias. Essas condições ainda precisam ser confirmadas pelo cliente.

## Fotos: sempre em estúdio
Todas as fotos usam o mesmo estúdio: fundo cinza quente sem emenda, softbox suave e roupas lisas sem logo de outra marca. Só o modelo muda. Os modelos são fictícios.

| Modelo | Perfil | Boné | Roupa lisa |
|---|---|---|---|
| A | Alto, loiro | Sombra Preto | Moletom off-white e calça preta |
| B | Negro, tranças | Sombra Marinho | Camiseta branca e bermuda jeans clara |
| C | Moreno, cacheado | Sombra Garrafa | Camiseta creme e jeans claro |
| D | Nipo-brasileiro, cabelo liso | Sombra Lavado | Camiseta cinza lavada e jeans preto desbotado |
| E | Negro, cabelo raspado, tatuagens finas | Sombra Osso | Moletom preto e calça preta |

Os prompts de foto seguem a skill `.claude/skills/sketch-to-studio-product`.

## Site
- `index.html` é o site inteiro, sem etapa de build. Os dados dos bonés ficam na lista `P` do script.
- Abertura do site: seção `#hero` com o vídeo `video/hero.mp4` (e `hero.webm`). O vídeo toca uma vez, sem som, e para no último quadro (o bordado "Headtuff" em macro); só então aparece a legenda no rodapé. Sobre o vídeo o menu fica transparente e sem logo. Em tela em pé (celular) o script troca para o vídeo vertical 9:16 `video/hero-celular.mp4`, em tela cheia. Cada vídeo tem o primeiro e o último quadro em WebP (`hero-inicio`/`hero-fim` e `hero-celular-inicio`/`hero-celular-fim`). Para trocar um vídeo, substituir o arquivo e os dois quadros dele.
- Fotos reais em `img/`, em WebP: `<boné>-packshot.webp` e `<boné>-modelo-N.webp` (até 1600 px de largura) e uma versão `-sm` de 640 px para cards e carrosséis. O objeto `IMG` no script diz quais fotos cada boné tem. Boné sem entrada em `IMG` (hoje o Sombra Flash) cai na ilustração SVG de reserva.
- Para adicionar foto: converter para WebP nas duas larguras, salvar em `img/` com esse padrão de nome e atualizar `IMG` (e a lista `LB` do lookbook, se for foto de modelo).
- Ordem das seções, inspirada no Wants and Needs: barra preta de aviso, menu com logo no centro, grade de produtos, banner "001 em breve", coleções ## Última tarefa concluída (13/11/2026)
Fotos reais no site: 19 imagens em `img/` (packshots de Preto, Osso, Marinho, Garrafa e Lavado; fotos de modelo de todos esses), fotos nos cards, carrossel no detalhe de cada boné e seção de lookbook. Ainda faltam todas as fotos do Sombra Flash.
