# LegalizaPro — Assessoria em Licenciamento e Regularização Empresarial

> Site institucional completo: landing page + portfólio de serviços em um único arquivo HTML. Foco em assessoria de licenciamento empresarial em todo o Brasil.

![Status](https://img.shields.io/badge/status-online-2EAD9F?style=flat-square)
![HTML](https://img.shields.io/badge/HTML5-puro-1E3A5F?style=flat-square&logo=html5)
![CSS](https://img.shields.io/badge/CSS3-responsivo-1E3A5F?style=flat-square&logo=css3)
![Deploy](https://img.shields.io/badge/deploy-Vercel-black?style=flat-square&logo=vercel)
![Domínio](https://img.shields.io/badge/domínio-legaliza.pro-2EAD9F?style=flat-square)

---

## 📋 Sobre o Projeto

A **LegalizaPro** é uma assessoria especializada em licenciamento e regularização empresarial com atuação nacional. Cuida de ponta a ponta da regularização de CNPJs, Inscrições Municipais, Alvarás de Funcionamento, AVCB, Publicidade, Taxas, EVTL, Matrículas de Imóveis e demais licenças exigidas por órgãos públicos em qualquer município do Brasil.

Este repositório contém o site institucional completo: **landing page + portfólio detalhado de serviços**, construído em um único arquivo HTML sem dependências externas.

---

## ✅ Funcionalidades do Site

- **6 abas de navegação** — Quem Somos, Serviços, Portfólio, Como Funciona, Preços e Contato
- **Portfólio interativo** — 7 categorias de serviços com accordion de escopo detalhado
- **Formulário de captação** — diagnóstico gratuito integrado ao Formspree
- **CTA de urgência** — destaque para casos de interdição e autuação com link direto ao WhatsApp
- **Botão WhatsApp flutuante** — acesso rápido em todas as páginas
- **100% responsivo** — desktop, tablet e celular
- **Deep links via hash** — ex: `legaliza.pro/#portfolio`, `legaliza.pro/#servicos`
- **Zero dependências** — HTML + CSS + JS puro, sem frameworks ou bibliotecas externas

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| **HTML5** | Estrutura semântica |
| **CSS3** | Estilos, animações e grid responsivo |
| **JavaScript Vanilla** | Abas, accordion e envio do formulário via AJAX |
| **Google Fonts — Inter** | Tipografia |
| **SVG inline** | Ícones sem dependências externas |
| **Formspree** | Recebimento de leads pelo formulário |

---

## 🚀 Como Usar

### Rodar Localmente

Não precisa instalar nada. Basta abrir o arquivo no navegador:

```bash
# 1. Clone o repositório
git clone https://github.com/SEU_USUARIO/legalizapro.git

# 2. Acesse a pasta
cd legalizapro

# 3. Abra no navegador
# Mac:
open index.html
# Windows (clique duplo no arquivo, ou no terminal):
start index.html
# Linux:
xdg-open index.html
```

> ⚠️ O formulário de contato só funciona quando acessado pelo site hospedado (não pelo arquivo local).

---

### 🌐 Deploy na Vercel

A Vercel hospeda o site gratuitamente com HTTPS automático, CDN global e deploy automático a cada `git push`.

**Via GitHub (recomendado):**

1. Acesse [vercel.com](https://vercel.com) e faça login com sua conta GitHub
2. Clique em **"Add New → Project"**
3. Selecione este repositório na lista
4. Clique em **"Deploy"** — pronto ✅

A cada `git push`, o site é atualizado automaticamente em ~30 segundos.

---

### 🔗 Domínio

O site está publicado em **[legaliza.pro](https://legaliza.pro)**, registrado no GoDaddy e apontado para a Vercel via registro DNS tipo `A`.

Para configurar outro domínio:
1. No painel da Vercel → **Settings → Domains**
2. Adicione o domínio desejado
3. Configure os registros DNS indicados pela Vercel no painel do registrador

---

## ✏️ Como Editar

Abra o `index.html` no [VS Code](https://code.visualstudio.com/) (gratuito) e use **Ctrl+F** para localizar e substituir os trechos abaixo.

### Informações de Contato

| Buscar | O que é |
|---|---|
| `5551998850289` | Número do WhatsApp (aparece em vários links) |
| `(51) 9 9885-0289` | Exibição do número (aparece 2×) |
| `comercial.legalizapro@gmail.com` | E-mail de contato (aparece 3×) |
| `legaliza.pro` | Domínio do site (aparece no footer e contato) |

### Textos Principais

| Buscar | O que é |
|---|---|
| `Regularização de licenças empresariais` | Título principal (hero) |
| `Cuidamos de toda a burocracia` | Subtítulo do hero |
| `A LegalizaPro nasceu para resolver` | Texto da seção "Quem Somos" |

### Formulário de Contato

O formulário está integrado ao Formspree (`xzdokzok`) via AJAX. Para trocar ou reconfigurar:

1. Acesse [formspree.io](https://formspree.io) e obtenha seu código de formulário
2. No `index.html`, localize dentro do script:

```js
const res = await fetch('https://formspree.io/f/xzdokzok', {
```

3. Substitua `xzdokzok` pelo seu código

---

## 📁 Estrutura do Repositório

```
legalizapro/
│
├── index.html        ← Site completo (único arquivo)
└── README.md         ← Este arquivo
```

O projeto é mantido em **arquivo único** para facilitar:
- Edição direta sem ambiente de desenvolvimento
- Deploy em qualquer hospedagem estática
- Histórico de versões limpo no Git

---

## 🎨 Paleta de Cores

Extraída do logo oficial da marca:

| Nome | Hex | Uso |
|---|---|---|
| **Navy** | `#1E3A5F` | Textos, headers, estrutura |
| **Teal** | `#2EAD9F` | CTAs, destaques, ícones ativos |
| **Teal Soft** | `#E8F7F4` | Fundos de cards e tags |
| **Off-white** | `#F8FAFC` | Seções alternadas |
| **Border** | `#E2E8F0` | Bordas e divisores |
| **Orange** | `#F97316` | CTAs de urgência (interdição) |

---

## 📌 Mapa de Seções

| Aba | Conteúdo |
|---|---|
| **Quem Somos** | Hero, card de urgência, stats de mercado, sobre a empresa, depoimentos |
| **Serviços** | 9 cards de serviços + 6 diferenciais competitivos |
| **Portfólio** | 7 sub-abas com escopo detalhado em accordion |
| **Como Funciona** | 4 passos do processo + 6 vantagens da terceirização |
| **Preços** | 2 modelos de contratação + FAQ com 6 perguntas |
| **Contato** | Canais de atendimento + formulário de captação de leads |

### Sub-abas do Portfólio

| Sub-aba | Serviços cobertos |
|---|---|
| CNPJ e Inscrição Municipal | Abertura, alteração, baixa de CNPJ e IM |
| Alvará de Funcionamento | ALF, provisório, definitivo, horário especial, desinterdição |
| Alvará de Bombeiros | AVCB, CLCB, PPCI, notificações urgentes |
| Alvará de Publicidade | Licença, formatação de projeto, vistoria técnica |
| Taxas, Débitos e Matrículas | Levantamento, regularização, certidões, matrículas de imóveis |
| Licenças e Certidões | Sanitária municipal/estadual, CNES, ambiental |
| EVTL e Viabilidade | Estudo de viabilidade, consulta prévia, análise pré-locação |

---

## 💰 Custos de Operação

| Item | Plataforma | Custo |
|---|---|---|
| Hospedagem | Vercel | **R$ 0** |
| Domínio `legaliza.pro` | GoDaddy | **~R$ 80/ano** |
| E-mail profissional | Gmail / Zoho Mail | **R$ 0** |
| Formulário de contato | Formspree | **R$ 0** (até 50 envios/mês) |
| **Total atual** | | **~R$ 6,70/mês** |

---

## 🔄 Workflow de Atualização

```
Editar index.html   →   Salvar   →   git add .   →   git commit -m "descrição"   →   git push
                                                                                          ↓
                                                                     Vercel republica automaticamente
                                                                     em ~30 segundos ✅
```

### Commits recomendados

```bash
git commit -m "fix: atualiza número de WhatsApp"
git commit -m "content: adiciona novo serviço ao portfólio"
git commit -m "fix: corrige texto do hero"
git commit -m "style: ajusta cores do card de urgência"
```

---

## 📬 Contato

**LegalizaPro — Assessoria em Licenciamento Empresarial**

- 🌐 [legaliza.pro](https://legaliza.pro)
- 📧 comercial.legalizapro@gmail.com
- 📱 (51) 9 9885-0289

---

## 📄 Licença

© 2025 LegalizaPro. Todos os direitos reservados.

Este repositório e seu conteúdo são de propriedade exclusiva da LegalizaPro e não podem ser reproduzidos, distribuídos ou utilizados sem autorização expressa.
