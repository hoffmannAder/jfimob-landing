# JF Imob — landing page (demo)

Landing page da **Jonas Farias Negócios Imobiliários** (Londrina/PR) com a estética
e as animações de referência da ogroup.com.

- Demo no ar: https://jfimob-landing.vercel.app
- Arquivo único: `index.html` (fotos embutidas em base64, sem build, sem servidor)

## Como abrir

Dois cliques em `index.html`, ou:

```bash
python3 -m http.server 8000
# http://localhost:8000
```

Precisa de internet só para as fontes (Google Fonts) e o GSAP (cdnjs).

## O que tem

- Preloader com monograma, hero fullscreen com slideshow Ken Burns e título revelado linha a linha
- Menu fullscreen (botão "+"), trilho social fixo, header que some ao descer e volta ao subir
- Busca funcional apontando para `jfimob.com.br/imoveis?q=&purpose=`
- Grid de imóveis com hover esmaecido, anel de pincel dourado e dados do imóvel
- Serviços com preview de foto no hover, bandas com parallax, contadores animados
- Seção do fundador com recorte real da foto e parallax de mouse em três profundidades
- Acesso rápido (IPTU, Copel, Sanepar), rodapé, pílula "Inteligência JF"
- `prefers-reduced-motion` respeitado: tudo estático, sem loader

## Conteúdo

Todos os textos, imóveis, preços, links e contatos vieram da página atual
(jfimob.com.br). Fotos dos imóveis: blob da Vercel do site atual, redimensionadas.

## Próximo passo sugerido

Converter para rota do Next.js do site atual e trocar as fotos base64 pelas URLs
do blob (o HTML cai de ~4,4 MB para ~30 KB).
