# Flavio AI Design System V3

![Version](https://img.shields.io/badge/version-1.0.0-orange)
![License](https://img.shields.io/badge/license-MIT-green)
![CSS](https://img.shields.io/badge/CSS-Design%20System-blue)

Sistema de design completo para a marca **Flavio AI** - democratizando inteligência artificial para designers e product managers não-técnicos através de transformação radical.

## 📚 Índice

- [Visão Geral](#-visão-geral)
- [Instalação](#-instalação)
- [Paletas de Cores](#-paletas-de-cores)
- [Componentes](#-componentes)
- [Exemplos](#-exemplos)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Guia de Uso](#-guia-de-uso)
- [Contribuindo](#-contribuindo)

## 🎯 Visão Geral

O **Flavio AI Design System V3** é um sistema de design modular e completo que inclui:

- ✅ **3 Paletas de Cores**: Equilibrada, Vibrante e Dark
- ✅ **Sistema de Espaçamento**: Baseado em múltiplos de 8px
- ✅ **Tipografia Escalável**: 8 tamanhos hierárquicos
- ✅ **50+ Componentes**: Botões, Cards, Forms, Modais e mais
- ✅ **Dark Mode Nativo**: Componentes otimizados para fundos escuros
- ✅ **Responsivo**: Mobile-first design
- ✅ **Font Awesome**: Biblioteca completa de ícones

## 🚀 Instalação

### Opção 1: CSS Direto (Recomendado)

```html
<!-- Font Awesome -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<!-- Flavio AI Design System -->
<link rel="stylesheet" href="path/to/src/css/flavio-ai-design-system.css">
```

### Opção 2: Importar CSS Individual

```html
<link rel="stylesheet" href="path/to/src/css/variables.css">
<link rel="stylesheet" href="path/to/src/css/base.css">
<link rel="stylesheet" href="path/to/src/css/buttons.css">
<link rel="stylesheet" href="path/to/src/css/cards.css">
<link rel="stylesheet" href="path/to/src/css/dark-components.css">
<link rel="stylesheet" href="path/to/src/css/components.css">
```

### Opção 3: Clone o Repositório

```bash
git clone https://github.com/seu-usuario/flavio-ai-design-system.git
cd flavio-ai-design-system
```

Abra `examples/showcase.html` ou `examples/landing-page.html` no navegador para ver os componentes em ação.

## 🎨 Paletas de Cores

### Paleta Equilibrada (Principal)

**Quando usar:** Conteúdo educacional, landing pages de conversão, apresentações de vendas

```css
--brand-primary:    #3A3A3C  /* Cinza Escuro - Base */
--brand-accent-1:   #E87A52  /* Coral Vibrante - Energia */
--brand-accent-2:   #388379  /* Verde Cerceta - Crescimento */
--brand-light:      #F5EFE7  /* Bege Claro - Respiração */
--brand-surface:    #5A5A5D  /* Cinza Médio - Profundidade */
```

### Paleta Vibrante (Alta Energia)

**Quando usar:** Campanhas de lançamento, CTAs de alta conversão, conteúdo viral

```css
--brand-vibrant-accent-1:   #FF6B35  /* Laranja Intenso */
--brand-vibrant-accent-2:   #2D9B87  /* Verde Água */
```

### Paleta Dark (Elegância Profunda)

**Quando usar:** Landing pages premium, conteúdo de consultoria enterprise, webinars

```css
--brand-dark-primary:    #1a1a1c  /* Preto Profundo */
--brand-dark-accent-1:   #D49479  /* Coral Suave */
--brand-dark-accent-2:   #4A6B6A  /* Verde Profundo */
```

## 📦 Componentes

### Botões

```html
<!-- Primary Button -->
<button class="btn btn-primary">
  <i class="fa-solid fa-rocket"></i> Primary Button
</button>

<!-- Secondary Button -->
<button class="btn btn-secondary">
  <i class="fa-solid fa-check"></i> Secondary Button
</button>

<!-- Outline Button -->
<button class="btn btn-outline">
  <i class="fa-solid fa-download"></i> Outline Button
</button>

<!-- Tamanhos -->
<button class="btn btn-primary btn-small">Small</button>
<button class="btn btn-primary">Regular</button>
<button class="btn btn-primary btn-large">Large</button>
<button class="btn btn-primary btn-xl">Extra Large</button>
```

### Cards Horizontais

```html
<!-- Card Light -->
<div class="card-horizontal light">
  <div class="card-icon">
    <i class="fa-solid fa-lightbulb"></i>
  </div>
  <div class="card-content">
    <h3 class="card-title">Título do Card</h3>
    <p class="card-text">Descrição do conteúdo...</p>
    <div class="card-actions">
      <span class="badge badge-primary">NOVO</span>
      <button class="btn btn-primary btn-small">Ação</button>
    </div>
  </div>
</div>

<!-- Card Dark -->
<div class="card-horizontal dark">
  <!-- Mesmo conteúdo com tema escuro -->
</div>

<!-- Card Accent -->
<div class="card-horizontal accent">
  <!-- Mesmo conteúdo com destaque -->
</div>
```

### Cards Verticais (Grid)

```html
<div class="cards-grid-3">
  <div class="card-vertical">
    <div class="card-icon">
      <i class="fa-solid fa-rocket"></i>
    </div>
    <h3 class="card-title">Título</h3>
    <p class="card-text">Descrição...</p>
    <div class="card-actions">
      <span class="badge badge-primary">TAG</span>
    </div>
  </div>
  <!-- Repetir para mais cards -->
</div>
```

### Hero Section Dark

```html
<div class="hero-dark">
  <div class="hero-content">
    <div class="hero-icon">
      <i class="fa-solid fa-wand-magic-sparkles"></i>
    </div>
    <h2>Título Impactante</h2>
    <p>Descrição persuasiva do valor...</p>
    <div style="display: flex; gap: 16px; justify-content: center;">
      <button class="btn btn-primary-dark btn-large">
        <i class="fa-solid fa-rocket"></i> CTA Principal
      </button>
      <button class="btn btn-outline-dark btn-large">
        <i class="fa-solid fa-play"></i> Ver Demo
      </button>
    </div>
  </div>
</div>
```

### Stats Grid

```html
<div class="stats-grid">
  <div class="stat-card">
    <div class="stat-value">500+</div>
    <div class="stat-label">Alunos Formados</div>
  </div>
  <div class="stat-card">
    <div class="stat-value secondary">85%</div>
    <div class="stat-label">Redução de Tempo</div>
  </div>
  <!-- Mais stats... -->
</div>
```

### Feature Cards Numeradas

```html
<div class="feature-card-dark">
  <div class="feature-number">1</div>
  <div class="feature-content">
    <h3>Título da Feature</h3>
    <p>Descrição detalhada...</p>
  </div>
</div>

<!-- Alternância de cores -->
<div class="feature-card-dark secondary">
  <div class="feature-number">2</div>
  <div class="feature-content">
    <h3>Segunda Feature</h3>
    <p>Descrição...</p>
  </div>
</div>
```

### Testimonials

```html
<div class="testimonial-dark">
  <i class="fa-solid fa-quote-right quote-icon"></i>
  <p class="testimonial-text">"Depoimento impactante do cliente..."</p>
  <div class="testimonial-author">
    <div class="author-avatar">
      <i class="fa-solid fa-user"></i>
    </div>
    <div class="author-info">
      <h4>Nome do Cliente</h4>
      <p>Cargo @ Empresa</p>
    </div>
  </div>
</div>
```

### Pricing Cards

```html
<div class="pricing-grid">
  <div class="pricing-card featured">
    <div class="pricing-badge">MAIS POPULAR</div>
    <div class="pricing-name">Professional</div>
    <div class="pricing-desc">Descrição do plano...</div>
    <div class="pricing-value">R$ 2.997</div>
    <div class="pricing-period">ou 12x de R$ 297</div>
    <ul class="pricing-features">
      <li>
        <i class="fa-solid fa-check"></i>
        <span>Feature incluída</span>
      </li>
      <!-- Mais features... -->
    </ul>
    <button class="btn btn-primary-dark" style="width: 100%;">
      Garantir Vaga
    </button>
  </div>
</div>
```

### Timeline Vertical

```html
<div class="timeline-dark">
  <div class="timeline-item">
    <div class="timeline-dot">
      <i class="fa-solid fa-rocket"></i>
    </div>
    <div class="timeline-content">
      <h3>Semana 1-2: Título</h3>
      <p>Descrição da etapa...</p>
    </div>
  </div>
  <!-- Mais itens alternando classes "secondary" -->
</div>
```

### Badges

```html
<span class="badge badge-primary">
  <i class="fa-solid fa-star"></i> NOVO
</span>
<span class="badge badge-secondary">
  <i class="fa-solid fa-fire"></i> EM ALTA
</span>
<span class="badge badge-light">DESTAQUE</span>
<span class="badge badge-dark">PREMIUM</span>
```

### Alert Boxes

```html
<!-- Info Alert -->
<div class="alert-dark info">
  <div class="alert-icon">
    <i class="fa-solid fa-circle-info"></i>
  </div>
  <div class="alert-content">
    <h4>Título do Alert</h4>
    <p>Mensagem informativa...</p>
  </div>
</div>

<!-- Variantes: success, warning, error -->
```

### Accordion / FAQ

```html
<div class="accordion-dark">
  <div class="accordion-header">
    <h3>Pergunta frequente?</h3>
    <i class="fa-solid fa-chevron-down accordion-icon"></i>
  </div>
  <div class="accordion-content">
    <p>Resposta detalhada...</p>
  </div>
</div>
```

### CTA Block

```html
<div class="cta-block">
  <h2>Título de Conversão</h2>
  <p>Proposta de valor clara...</p>
  <div class="btn-group center">
    <button class="btn btn-light btn-xl">
      <i class="fa-solid fa-rocket"></i> CTA Principal
    </button>
  </div>
  <div class="urgency-text">
    <i class="fa-solid fa-clock"></i>
    <span>Urgência e garantia...</span>
  </div>
</div>
```

## 🎬 Exemplos

### Showcase Completo

Abra `examples/showcase.html` para ver todos os componentes em ação com exemplos de uso.

### Landing Page de Conversão

Abra `examples/landing-page.html` para ver um exemplo completo de landing page seguindo as melhores práticas:

1. ✅ Hero Section Dark com CTAs
2. ✅ Social Proof (Stats)
3. ✅ Features Numeradas
4. ✅ Casos de Uso / Resultados
5. ✅ Testimonials
6. ✅ Pricing com 3 tiers
7. ✅ FAQ (Accordion)
8. ✅ CTA Final com Urgência

## 📁 Estrutura do Projeto

```
flavio-ai-design-system/
├── src/
│   └── css/
│       ├── variables.css           # Variáveis CSS e tokens
│       ├── base.css                # Reset e estilos base
│       ├── buttons.css             # Componentes de botões
│       ├── cards.css               # Sistema de cards
│       ├── dark-components.css     # Componentes dark mode
│       ├── components.css          # Componentes adicionais
│       └── flavio-ai-design-system.css  # Entry point (import all)
├── examples/
│   ├── showcase.html               # Demonstração completa
│   └── landing-page.html           # Exemplo de landing page
├── docs/                           # Documentação adicional
└── README.md                       # Este arquivo
```

## 🎓 Guia de Uso

### Sistema de Espaçamento

Use sempre múltiplos de **8px** para consistência:

```css
--space-xs:  8px   /* Micro espaços */
--space-sm:  16px  /* Elementos próximos */
--space-md:  24px  /* Separação padrão */
--space-lg:  32px  /* Seções relacionadas */
--space-xl:  48px  /* Grandes blocos */
--space-2xl: 64px  /* Seções distintas */
--space-3xl: 96px  /* Quebras dramáticas */
```

### Tipografia

```css
/* Display */
--text-4xl: 48px   /* Hero sections */
--text-3xl: 36px   /* H1, títulos principais */
--text-2xl: 28px   /* H2, subtítulos */
--text-xl:  22px   /* H3, cards destacados */

/* Body */
--text-lg:   18px  /* Parágrafos de destaque */
--text-base: 16px  /* Corpo padrão */
--text-sm:   14px  /* Labels, metadados */
--text-xs:   12px  /* Footnotes */
```

### Classes Utilitárias

```html
<!-- Spacing -->
<div class="mt-xl mb-2xl py-lg">...</div>

<!-- Text -->
<p class="text-center font-bold">...</p>

<!-- Flexbox -->
<div class="flex items-center justify-between gap-md">...</div>

<!-- Container -->
<div class="container">...</div>
<div class="container container-narrow">...</div>
```

### Responsividade

Todos os componentes são responsivos por padrão. Breakpoints:

```css
--screen-sm:  640px   /* Mobile landscape */
--screen-md:  768px   /* Tablet */
--screen-lg:  1024px  /* Desktop */
--screen-xl:  1280px  /* Large desktop */
--screen-2xl: 1536px  /* Extra large */
```

## 🎯 Princípios do Design System

### Tom de Voz

**USE sempre:**
- Transformação (não "melhoria")
- Exponencial (não "incremental")
- Democratizar (não "facilitar")
- Revolucionar (não "otimizar")

**EVITE sempre:**
- Buzzwords vazios: "disruptivo", "inovação"
- Jargão técnico desnecessário
- Promessas mágicas irrealistas
- Linguagem corporativa fria

### Framework de Mensagens

Para landing pages e conteúdo de conversão:

1. **HOOK** - Problema real + impacto emocional
2. **EXEMPLO** - Caso concreto + números
3. **INSIGHT** - Mudança de paradigma
4. **AÇÃO** - Caminho claro + urgência

### Anatomia de Landing Page

1. Hero Section (Dark) com ícone + 2 CTAs
2. Social Proof (Stats Grid Light)
3. Features Numeradas (Dark)
4. Testimonials (Dark, alternando bordas)
5. Pricing (Dark, 3 cards com featured)
6. FAQ (Accordion Dark)
7. CTA Final (Gradient)

## 🚀 Deploy com GitHub Pages

Para publicar a documentação:

1. Crie um arquivo `index.html` na raiz ou configure `docs/` folder
2. Vá em Settings → Pages
3. Selecione branch `main` e folder `/` ou `/docs`
4. Acesse em: `https://seu-usuario.github.io/nome-do-repo`

**Exemplo de index.html:**

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="refresh" content="0; url=examples/showcase.html">
  <title>Flavio AI Design System</title>
</head>
<body>
  Redirecionando para showcase...
</body>
</html>
```

## 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/NovaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona NovaFeature'`)
4. Push para a branch (`git push origin feature/NovaFeature`)
5. Abra um Pull Request

### Convenções

- Use BEM para nomenclatura CSS quando aplicável
- Mantenha espaçamento baseado em 8px
- Teste em mobile, tablet e desktop
- Documente novos componentes no showcase.html

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 📞 Suporte

- **Documentação:** [GitHub Pages](https://seu-usuario.github.io/flavio-ai-design-system)
- **Issues:** [GitHub Issues](https://github.com/seu-usuario/flavio-ai-design-system/issues)
- **Email:** contato@flavioai.com

---

**Versão:** 1.0.0
**Última atualização:** Janeiro 2025
**Baseado em:** Design System V3 + V3 Dark Extended

<div align="center">
  <strong>Democratizando IA para designers e PMs não-técnicos</strong>
</div>
