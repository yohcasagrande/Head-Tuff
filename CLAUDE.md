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
- `index.html` é o site inteiro, sem etapa de build. Os bonés hoje são ilustrações em SVG geradas pelo script do próprio arquivo (lista `P`).
- Ordem das seções, inspirada no Wants and Needs: barra preta de aviso, menu com logo no centro, grade de produtos, banner "001 em breve", coleções 01/02/03, banner "Cabeça dura", carrossel "001 Todos os produtos", Instagram, faixa de promessas e rodapé.
- Ainda não há carrinho. Todo botão de compra leva ao Direct do Instagram (`https://ig.me/m/useheadtuff`).
- **Publicação:** projeto `headtuff` na Vercel, ligado a este repositório. Cada envio para a branch `main` vai ao ar sozinho em headtuff.com. O `.vercelignore` impede que a pasta `.claude` e o README sejam publicados.

## Próxima tarefa
O usuário tem uma pasta **HeadTuff** no computador com as imagens geradas: fotos dos bonés e fotos dos modelos usando os bonés. Pedido:

1. Copiar as imagens para `img/` neste repositório, com nomes claros, como `preto-packshot.webp` e `preto-modelo-1.webp`. Converter para WebP com largura máxima de cerca de 1600 px, para o site carregar rápido.
2. Trocar as ilustrações SVG pelas fotos reais nos cards de produto e no detalhe do produto.
3. Na janela de detalhe de cada boné, colocar um **carrossel** com o packshot e as fotos do modelo correspondente.
4. Criar no site uma seção de **lookbook em carrossel** com os modelos usando os bonés.
5. Manter as ilustrações SVG como reserva para os bonés que ainda não têm foto, como o Sombra Flash.
6. Conferir no computador e no celular, fazer commit e enviar para a `main`. Depois, confirmar que headtuff.com atualizou.
