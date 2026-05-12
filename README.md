# LegalizaPro — Licenciamento Empresarial | Alvará, AVCB e EVTL

> Site institucional completo: landing page + portfólio detalhado de serviços em um único arquivo HTML. Foco em assessoria especializada em licenciamento e regularização empresarial com atuação nacional.

![Status](https://img.shields.io/badge/status-online-2EAD9F?style=flat-square)
![HTML](https://img.shields.io/badge/HTML5-puro-1E3A5F?style=flat-square&logo=html5)
![CSS](https://img.shields.io/badge/CSS3-responsivo-1E3A5F?style=flat-square&logo=css3)
![Deploy](https://img.shields.io/badge/deploy-Vercel-black?style=flat-square&logo=vercel)
![Domínio](https://img.shields.io/badge/domínio-legaliza.pro-2EAD9F?style=flat-square)
![Analytics](https://img.shields.io/badge/analytics-G--GM9HKEXW94-orange?style=flat-square&logo=googleanalytics)

---

## 📋 Sobre o Projeto

A **LegalizaPro** é uma assessoria especializada em licenciamento e regularização empresarial com atuação nacional — CNPJ, Inscrição Municipal, Alvará de Localização e Funcionamento, AVCB, CLCB, Publicidade, Taxas, EVTL e Matrículas de Imóveis em qualquer município do Brasil.

Este repositório contém o site institucional completo: **landing page + portfólio de serviços integrados** em sistema de abas interativo, construído em arquivo único sem dependências externas.

---

## ✅ Funcionalidades

- **6 abas de navegação** — Quem Somos, Serviços, Portfólio, Como Funciona, Preços e Contato
- **Cases de sucesso** — Métricas reais: +10.000 processos, +1.000 CNPJs, +3.000 EVTLs, +9 anos de experiência
- **Portfólio interativo** — 7 categorias com accordion de escopo detalhado
- **Projetos estratégicos** — Expansão e migração, Due Diligence regulatória, Governança e KPIs
- **Formulário de captação** — AJAX via Formspree, sem redirect, com mensagem de sucesso inline
- **CTA de urgência** — Card laranja para interdição/autuação com link direto ao WhatsApp
- **Botão WhatsApp flutuante** — acesso rápido em todas as seções
- **100% responsivo** — desktop, tablet e celular
- **Deep links via hash** — `legaliza.pro/#servicos`, `legaliza.pro/#portfolio`, etc.
- **Zero dependências** — HTML + CSS + JS vanilla, sem frameworks

---

## 🔍 SEO — Implementado

| Elemento | Detalhe |
|---|---|
| **Title** | `LegalizaPro — Licenciamento Empresarial \| Alvará, AVCB e EVTL` (61 chars) |
| **Meta description** | 151 chars — dentro do limite do Google |
| **Meta keywords** | 12 termos-chave do setor |
| **Canonical URL** | `https://legaliza.pro` |
| **Open Graph** | title, description, image, type, locale, alt, dimensions |
| **Twitter Card** | `summary_large_image` — sincronizado com og:title |
| **JSON-LD Schema** | ProfessionalService + FAQPage + WebSite + ItemList |
| **Google Analytics** | `G-GM9HKEXW94` |
| **Favicon** | SVG inline — sem arquivo externo |
| **noscript** | Conteúdo das abas visível para Googlebot sem JS |
| **DNS prefetch** | Google Fonts com preconexão otimizada |
| **noopener noreferrer** | Todos os links externos protegidos |
| **Footer âncoras** | `href="#servicos"`, `href="#portfolio"` etc. |
| **og:image** | `og-image.jpg` — 1200×630px com tagline "Regularize. Proteja. Cresça." |

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| **HTML5** | Estrutura semântica |
| **CSS3** | Estilos, animações e grid responsivo |
| **JavaScript Vanilla** | Abas, accordion, envio AJAX do formulário |
| **Google Fonts — Inter** | Tipografia principal |
| **SVG inline** | Ícones sem dependências externas |
| **Formspree** | Recebimento de leads (`xzdokzok`) |
| **Google Analytics 4** | Rastreamento de eventos e conversões |

---

## 🚀 Como Usar

### Rodar Localmente

```bash
# 1. Clone o repositório
git clone https://github.com/SEU_USUARIO/legalizapro.git

# 2. Acesse a pasta
cd legalizapro

# 3. Abra no navegador
open index.html          # Mac
start index.html         # Windows
xdg-open index.html      # Linux
```

> ⚠️ O formulário e o Analytics só funcionam no site hospedado (não local).

---

### 🌐 Deploy (Vercel — automático)

A Vercel republica o site automaticamente a cada `git push`.

1. Acesse [vercel.com](https://vercel.com) → login com GitHub
2. **Add New → Project** → selecione este repositório
3. Clique em **Deploy** ✅

---

### 🔗 Domínio

Registrado no **GoDaddy**: `legaliza.pro`
Apontado via registro DNS tipo **A → 216.198.79.1** para a Vercel.

| Domínio | Status |
|---|---|
| `legaliza.pro` | ✅ Produção (domínio principal) |
| `legalizapro.vercel.app` | ✅ Redireciona 308 → `legaliza.pro` |

---

## ✏️ Como Editar

Abra o `index.html` no [VS Code](https://code.visualstudio.com) e use **Ctrl+F** para localizar:

### Informações de contato

| Buscar | O que é |
|---|---|
| `5551998850289` | Número no WhatsApp (links) |
| `(51) 9 9885-0289` | Número exibido no site |
| `comercial.legalizapro@gmail.com` | E-mail de contato |
| `legaliza.pro` | Domínio |

### Cases de sucesso (números)

| Buscar | O que é |
|---|---|
| `+10.000` | Processos de regularização realizados |
| `+1.000` | CNPJs viabilizados |
| `+3.000` | EVTLs realizados |
| `+9 anos` | Anos de experiência |

### Hero e textos principais

| Buscar | O que é |
|---|---|
| `Regularização de` | Início do H1 principal |
| `Cuidamos de toda a legalização` | Subtítulo do hero |
| `Empresa autuada ou sem alvará?` | Card de urgência laranja |
| `A LegalizaPro nasceu para` | Texto da seção Quem Somos |

### Formulário de contato

O formulário usa Formspree via AJAX. Para trocar o endpoint:

```js
// Localize no <script> ao final do arquivo:
const res = await fetch('https://formspree.io/f/xzdokzok', {
// Substitua "xzdokzok" pelo seu código Formspree
```

### Google Analytics

```html
<!-- Localize no <head>: -->
gtag('config', 'G-GM9HKEXW94');
<!-- Substitua pelo seu ID de medição -->
```

### Google Search Console

```html
<!-- Localize o placeholder no <head>: -->
<!-- SUBSTITUIR: cole aqui a meta tag de verificação do Google Search Console -->
<!-- <meta name="google-site-verification" content="SEU_CODIGO_AQUI"> -->
```

---

## 📁 Estrutura do Repositório

```
legalizapro/
│
├── index.html        ← Site completo (único arquivo — 3.027 linhas, ~126KB)
├── og-image.jpg      ← Imagem para compartilhamento social (1200×630px)
├── sitemap.xml       ← Mapa do site para o Google
├── robots.txt        ← Instruções para robôs de busca
└── README.md         ← Este arquivo
```

---

## 🎨 Identidade Visual

| Nome | Hex | Uso |
|---|---|---|
| **Navy** | `#1E3A5F` | Textos, headers, estrutura |
| **Teal** | `#2EAD9F` | CTAs, destaques, ícones |
| **Teal Soft** | `#E8F7F4` | Fundos de cards e tags |
| **Orange** | `#F97316` | CTAs de urgência (interdição) |
| **Off-white** | `#F8FAFC` | Seções alternadas |
| **Border** | `#E2E8F0` | Bordas e divisores |

**Tagline:** REGULARIZE. PROTEJA. CRESÇA.

---

## 📌 Mapa de Seções

| Aba | Hash | Conteúdo |
|---|---|---|
| **Quem Somos** | `#quem-somos` | Hero, card urgência, stats, sobre a empresa, cases de sucesso |
| **Serviços** | `#servicos` | 9 cards de serviços + 6 diferenciais |
| **Portfólio** | `#portfolio` | 7 sub-abas com accordion detalhado |
| **Como Funciona** | `#como-funciona` | 4 passos + projetos estratégicos + 6 vantagens |
| **Preços** | `#precos` | 2 modelos de contratação + FAQ |
| **Contato** | `#contato` | Canais + formulário de captação |

### Sub-abas do Portfólio

| Sub-aba | Hash | Serviços cobertos |
|---|---|---|
| CNPJ e Inscrição Municipal | `pc-cnpj` | Abertura, alteração, regularização e baixa |
| Alvará de Funcionamento | `pc-alvara` | ALF, provisório, definitivo, desinterdição |
| Alvará de Bombeiros | `pc-bombeiros` | AVCB, CLCB, PPCI, urgências |
| Alvará de Publicidade | `pc-publicidade` | Licença, projeto, vistoria técnica |
| Taxas, Débitos e Matrículas | `pc-taxas` | Levantamento, regularização, certidões, matrículas |
| Licenças e Certidões | `pc-licencas` | Sanitária municipal/estadual, CNES, ambiental |
| EVTL e Viabilidade | `pc-evtl` | Estudo de viabilidade, consulta prévia |

---

## 💰 Custos de Operação

| Item | Plataforma | Custo |
|---|---|---|
| Hospedagem | Vercel | **R$ 0** |
| Domínio `legaliza.pro` | GoDaddy | **~R$ 80/ano** |
| E-mail | Gmail | **R$ 0** |
| Formulário | Formspree | **R$ 0** (até 50/mês) |
| Analytics | Google Analytics 4 | **R$ 0** |
| **Total** | | **~R$ 6,70/mês** |

---

## 🔄 Workflow de Atualização

```
Editar index.html  →  Ctrl+S  →  Testar no navegador
        ↓
git add .  →  git commit -m "descrição"  →  git push
        ↓
Vercel republica automaticamente em ~30 segundos ✅
        ↓
Verificar em legaliza.pro (aba anônima, Ctrl+F5)
```

---

## 📊 Monitoramento

| Ferramenta | URL | Para quê |
|---|---|---|
| **Google Analytics** | [analytics.google.com](https://analytics.google.com) | Visitas, eventos, origem do tráfego |
| **Google Search Console** | [search.google.com/search-console](https://search.google.com/search-console) | Indexação, palavras-chave, erros |
| **Vercel Analytics** | [vercel.com/dashboard](https://vercel.com/dashboard) | Performance e deploys |

---

## 📬 Contato

**LegalizaPro — Regularize. Proteja. Cresça.**

- 🌐 [legaliza.pro](https://legaliza.pro)
- 📧 comercial.legalizapro@gmail.com
- 📱 (51) 9 9885-0289

---

## 📄 Licença

© 2025 LegalizaPro. Todos os direitos reservados.

Este repositório e seu conteúdo são de propriedade exclusiva da LegalizaPro e não podem ser reproduzidos, distribuídos ou utilizados sem autorização expressa.
