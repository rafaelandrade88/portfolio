# Portfólio — Rafael Andrade

Site pessoal e vitrine de serviços. Construído para converter visitantes em clientes — com proposta de valor clara, processo transparente e uma demonstração ao vivo de IA integrada.

**Acesse:** https://randradedev.netlify.app/

---

## Sobre

Portfólio construído como arquivo HTML único — sem frameworks, sem dependências externas, sem processo de build. Abre no navegador, funciona em qualquer dispositivo, faz deploy em segundos.

A estrutura foi revisada para funcionar como uma landing page de serviços, não apenas como currículo visual. Cada seção serve a um objetivo de conversão específico.

---

## Seções

| Seção | Objetivo |
|---|---|
| **Hero** | Comunicar a proposta de valor em 5 segundos |
| **Projetos** | Demonstrar capacidade técnica com produtos reais em produção |
| **Como trabalho** | Eliminar incerteza — 4 etapas com prazo estimado |
| **Serviços** | Detalhar o que pode ser contratado e o que está incluso |
| **Sobre** | Credenciais, stack e contexto profissional |
| **Contato** | Converter o visitante em lead |
| **Chat IA** | Demo ao vivo de integração com IA (widget flutuante) |

---

## Projetos apresentados

| Projeto | Descrição | Stack |
|---|---|---|
| [Bíblia Sagrada](https://appbibliasagrada.netlify.app/biblia-sagrada.html) | PWA offline com a Bíblia completa em português | HTML, JS, Service Worker, IndexedDB |
| [PaceRun](https://pacerun.netlify.app/) | App de corrida com GPS e análise por IA | Leaflet.js, Firebase, Claude AI |
| [GymFlow](https://gymflowfit.netlify.app/) | Tracker de treinos com sync em nuvem | Firebase, Firestore, Cloudinary, Charts.js |
| [FinanceFlow](https://appfinancasflow.netlify.app/) | Controle financeiro pessoal e familiar | Firebase, Firestore, Chart.js |
| [Copa do Mundo 2026](https://copadomundo26.streamlit.app/) | Dashboard interativo da Copa 2026 | Python, Streamlit, Pandas, Plotly |

---

## Serviços disponíveis

| Serviço | O que inclui | Prazo médio |
|---|---|---|
| **App Web + IA** | PWA, auth, banco de dados em tempo real, Claude/OpenAI integrado, deploy | ~14 dias |
| **Automação Inteligente** | Workflows n8n, webhooks, integrações com APIs, IA para triagem e classificação | ~7 dias |
| **Dashboard de Dados** | Python + Streamlit + Plotly, filtros interativos, KPIs, deploy em nuvem | ~10 dias |

---

## Destaques técnicos do site

**Visual**
- Starfield com 280 estrelas animadas em canvas — paralaxe responsiva ao mouse com 3 camadas de profundidade
- Glassmorphism nos cards com `backdrop-filter: blur()` e accent color individual por projeto
- Cursor glow seguindo o ponteiro
- Névoa de nebulosa com gradientes radiais em camadas fixas
- Scroll reveal progressivo via `IntersectionObserver`
- Menu hamburguer animado com overlay fullscreen em mobile

**Performance**
- Constellation lines otimizadas: 40 estrelas (era 60), comparação por distância quadrática no lugar de `Math.hypot`
- `prefers-reduced-motion`: desliga todas as animações e o canvas para usuários que precisam

**Acessibilidade**
- `aria-hidden` em todos os elementos decorativos (canvas, nebula, cursor glow)
- `focus-visible` com outline em cyan para navegação por teclado
- `role="dialog"` e `aria-label` no widget de chat
- Contraste de texto muted elevado para passar ratio 3:1 (WCAG AA)

**SEO**
- Open Graph completo (título, descrição, tipo, URL)
- Twitter Card configurado
- Favicon SVG inline com as iniciais `ra`

**Widget de Chat**
- Painel flutuante com header, chips de perguntas e campo de texto livre
- Pattern matching por regex para 5 intenções (serviços, prazo, preço, tecnologias, IA)
- Typewriter effect nas respostas (14ms/char)
- Delay simulado para naturalidade (700–1000ms)
- Responsivo em mobile

---

## Tecnologias

| Camada | Tecnologia |
|---|---|
| Estrutura | HTML5 semântico |
| Estilo | CSS3 — custom properties, grid, clamp(), backdrop-filter, keyframes |
| Interação | JavaScript vanilla — Canvas API, IntersectionObserver, DOM |
| Tipografia | Space Grotesk (display) · Inter (corpo) · Space Mono (mono) via Google Fonts |
| Deploy | Netlify — CD automático a partir da branch `main` |

Zero dependências. Zero npm install. Zero processo de build.

---

## Responsividade

| Breakpoint | Comportamento |
|---|---|
| `> 1280px` | Desktop — layout completo, 3 colunas de cards |
| `≤ 1280px` | Container reduzido para 960px |
| `≤ 1024px` | 2 colunas de cards, process grid em 2×2 |
| `≤ 768px` | Coluna única, nav com hamburguer, contact links empilhados |
| `≤ 480px` | Mobile — tipografia e espaçamentos comprimidos, chat widget full-width |

---

## Como rodar localmente

Não precisa de servidor. Basta abrir o arquivo:

```bash
git clone https://github.com/rafaelandrade88/portfolio.git
cd portfolio

# macOS / Linux
open index.html

# Windows
start index.html
```

---

## Estrutura

```
portfolio/
├── index.html    # Aplicação completa — HTML + CSS + JS em arquivo único
└── README.md
```

---

Desenvolvido por **Rafael Andrade** 
