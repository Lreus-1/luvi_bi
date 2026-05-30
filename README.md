# LUVI BI — Portfólio de Consultoria Power BI

Landing page de portfólio da **LUVI BI**, com dashboards interativos de Power BI incorporados diretamente na página.

## 🚀 Deploy

Hospedado no [Vercel](https://vercel.com) via site estático.

## 📊 Painéis disponíveis

| Painel | Área | Descrição |
|---|---|---|
| Relatório de Vendas | Comercial | Faturamento, ticket médio, ranking de produtos e vendedores |
| Dashboard Financeiro | Financeiro | DRE automatizado, margem líquida, custos por categoria |
| Controle de Estoque | Operações | Entradas, saídas, giro de estoque por produto e período |

## 🗂️ Estrutura do projeto

```
/
├── index.html      # Página principal com os iframes do Power BI
├── vercel.json     # Configuração de deploy e headers de segurança
└── README.md       # Este arquivo
```

## ⚙️ Como funciona

- A página é 100% estática — apenas HTML, CSS e JavaScript puro
- Os relatórios do Power BI são incorporados via `<iframe>` com os links públicos de "Publicar na web"
- Lazy loading: os iframes de Financeiro e Estoque só carregam ao clicar na aba correspondente, mantendo a página rápida
- Cada painel tem botão "Abrir em tela cheia" que leva ao Power BI Service

## 🛠️ Tecnologias

- HTML5 / CSS3 / JavaScript vanilla
- [Google Fonts — Sora + DM Serif Display](https://fonts.google.com)
- Power BI Embed (links públicos)
- Vercel (hospedagem estática gratuita)

## 📝 Como atualizar os relatórios

Para trocar um link de relatório, abra o `index.html` e localize a variável correspondente:

```html
<!-- Vendas -->
<iframe src="https://app.powerbi.com/view?r=SEU_LINK_AQUI" ...>

<!-- Financeiro -->
<iframe data-src="https://app.powerbi.com/view?r=SEU_LINK_AQUI" ...>

<!-- Estoque -->
<iframe data-src="https://app.powerbi.com/view?r=SEU_LINK_AQUI" ...>
```

## 📞 Contato

Para atualizar os dados de contato (WhatsApp e e-mail), localize no `index.html`:

```html
<a href="https://wa.me/5500000000000" ...>
<a href="mailto:contato@luvibi.com.br" ...>
```

---

Desenvolvido por **LUVI BI** · Consultoria Power BI & Dados
