# LegalizaPro — Compliance Empresarial Inteligente

> Plataforma de gestão regulatória para empresas brasileiras. Landing page + portfólio de serviços em um único arquivo HTML.

![Status](https://img.shields.io/badge/status-online-2EAD9F?style=flat-square)
![HTML](https://img.shields.io/badge/HTML5-puro-1E3A5F?style=flat-square&logo=html5)
![CSS](https://img.shields.io/badge/CSS3-responsivo-1E3A5F?style=flat-square&logo=css3)
![Deploy](https://img.shields.io/badge/deploy-Vercel-black?style=flat-square&logo=vercel)

---

## 📋 Sobre o Projeto

A **LegalizaPro** é uma plataforma de compliance empresarial que simplifica a gestão regulatória de empresas no Brasil — alvarás, licenças, AVCB, vigilância sanitária, licença ambiental, gestão documental e facilities.

Este repositório contém o site institucional completo: **landing page + portfólio de serviços** integrados em um sistema de abas interativo, sem dependências externas.

---

## ✅ Funcionalidades

- **6 abas de navegação** — Quem Somos, Produto, Portfólio, Como Funciona, Preços e Contato
- **Portfólio interativo** — 8 categorias de serviços com accordion de escopo detalhado
- **Dashboard mockup** — visualização do sistema de compliance em tempo real
- **Formulário de captação** — diagnóstico gratuito com campos qualificadores
- **100% responsivo** — funciona em desktop, tablet e celular
- **Deep links via hash** — ex: `legalizapro.com.br/#portfolio`
- **Zero dependências** — HTML + CSS + JS puro, sem frameworks ou bibliotecas externas

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| **HTML5** | Estrutura semântica |
| **CSS3** | Estilos, animações e grid responsivo |
| **JavaScript Vanilla** | Abas, accordion e navegação |
| **Google Fonts — Inter** | Tipografia |
| **SVG inline** | Ícones sem dependências externas |

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

---

### 🌐 Deploy na Vercel (Recomendado — Grátis)

A Vercel oferece hospedagem gratuita com HTTPS automático e CDN global.

**Via GitHub (mais prático — atualiza automaticamente a cada push):**

1. Acesse [vercel.com](https://vercel.com) e faça login com sua conta GitHub
2. Clique em **"Add New → Project"**
3. Selecione **este repositório** na lista
4. Clique em **"Deploy"** — pronto ✅

A cada `git push` que você fizer, o site é atualizado automaticamente.

**Via upload direto:**

1. Acesse [vercel.com/new](https://vercel.com/new)
2. Arraste a pasta do projeto na área indicada
3. Clique em **"Deploy"**

---

### 🔗 Conectar Domínio Próprio

Após o deploy na Vercel:

1. No painel do projeto, vá em **Settings → Domains**
2. Digite seu domínio (ex: `legalizapro.com.br`) e clique em **Add**
3. A Vercel exibirá dois registros DNS para configurar
4. Acesse o painel do seu registrador (ex: [Registro.br](https://registro.br)) e adicione esses registros
5. Aguarde até 4 horas para propagar

---

## ✏️ Como Editar

Abra o `index.html` em qualquer editor de texto. Recomendamos o [VS Code](https://code.visualstudio.com/) (gratuito).

Use **Ctrl+F** no editor para localizar os trechos abaixo e substituir:

### Informações de Contato

| Buscar | Substituir por |
|---|---|
| `(11) 9 0000-0000` | Seu número real (aparece 2×) |
| `contato@legalizapro.com.br` | Seu e-mail real (aparece 3×) |
| `www.legalizapro.com.br` | Seu domínio real (aparece 3×) |
| `https://wa.me/5511000000000` | Seu link do WhatsApp |

### Textos Principais

| Buscar | O que é |
|---|---|
| `Sua empresa sempre` | Título principal do hero |
| `Diagnóstico automático, alertas` | Subtítulo do hero |
| `A LegalizaPro nasceu da` | Texto "Quem Somos" |

### Preços

| Buscar | O que é |
|---|---|
| `297` | Preço do plano Profissional |
| `697` | Preço do plano Corporativo |

---

### 📬 Ativar o Formulário de Contato

O formulário exibe um alerta de confirmação por padrão. Para receber as mensagens no seu e-mail:

**Usando o Formspree (grátis até 50 mensagens/mês):**

1. Crie conta em [formspree.io](https://formspree.io)
2. Crie um novo formulário e copie o código gerado (ex: `xrgwabcd`)
3. No `index.html`, localize esta linha:

```html
<form class="contact-form" onsubmit="event.preventDefault(); alert('Mensagem enviada! ...
```

4. Substitua por:

```html
<form class="contact-form" action="https://formspree.io/f/SEU_CODIGO" method="POST">
```

5. Salve, faça o commit e o push — o formulário passará a enviar para seu e-mail

---

## 📁 Estrutura do Repositório

```
legalizapro/
│
├── index.html        ← Site completo (único arquivo)
└── README.md         ← Este arquivo
```

O projeto foi intencionalmente mantido em **arquivo único** para facilitar:
- Edição direta sem ambiente de desenvolvimento complexo
- Deploy em qualquer hospedagem estática
- Histórico de versões simples no Git

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

---

## 📌 Mapa de Seções

| Aba | Conteúdo |
|---|---|
| **Quem Somos** | Hero com stats de mercado, apresentação institucional, missão/visão/valores |
| **Produto** | 6 funcionalidades da plataforma, mockup do dashboard, benefícios |
| **Portfólio** | 8 categorias de serviços com escopo detalhado em accordion |
| **Como Funciona** | 4 passos do processo + 6 diferenciais competitivos |
| **Preços** | 4 planos (Starter, Profissional, Corporativo, White Label) + modalidades |
| **Contato** | Canais de atendimento + formulário de captação de leads |

---

## 💰 Custos de Operação

| Item | Plataforma | Custo |
|---|---|---|
| Hospedagem | Vercel | **R$ 0** |
| Domínio `.com.br` | Registro.br | **~R$ 40/ano** |
| E-mail profissional | Zoho Mail | **R$ 0** (até 5 usuários) |
| Formulário de contato | Formspree | **R$ 0** (até 50/mês) |
| **Total mínimo** | | **~R$ 3,30/mês** |

---

## 🔄 Workflow de Atualização

```
Editar index.html   →   Salvar   →   git add .   →   git commit   →   git push
                                                                           ↓
                                                              Vercel detecta e republica
                                                              automaticamente em ~30s ✅
```

---

## 📬 Contato

**LegalizaPro — Compliance Empresarial Inteligente**

- 🌐 [legalizapro.com.br](https://legalizapro.com.br)
- 📧 contato@legalizapro.com.br
- 📱 (11) 9 0000-0000

---

## 📄 Licença

© 2026 LegalizaPro. Todos os direitos reservados.

Este repositório e seu conteúdo são de propriedade exclusiva da LegalizaPro e não podem ser reproduzidos, distribuídos ou utilizados sem autorização expressa.
