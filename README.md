# LUVI BI — site

Página única em HTML estático (sem build), publicada na Vercel (`vercel.json`).

## Estrutura

```
index.html      página completa (textos, estilos da página e iframes do Power BI)
assets/         kit visual (CSS e JS), não editar
img/            logo e imagens dos painéis
share.jpg       imagem de pré-visualização ao compartilhar o link
original/       site anterior, guardado como referência
```

## Como atualizar

- **Painéis do Power BI:** em `index.html`, seção `#paineis`, troque o link `https://app.powerbi.com/view?r=...`
  no `href` de cada linha e no `data-src` do `iframe` correspondente.
  Para telas pequenas, as imagens `img/painel-*-m.png` mostram cada painel no lugar do iframe; atualize-as se o painel mudar muito.
- **WhatsApp e e-mail:** procure por `wa.me` e `mailto:` no `index.html`.
- **Domínio:** quando houver domínio próprio, descomente a linha `rel="canonical"` no `<head>`.

Desenvolvido por **LUVI BI** · Consultoria Power BI & Dados
