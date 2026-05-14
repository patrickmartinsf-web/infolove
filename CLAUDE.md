# Patrick & Camila — Infográfico WhatsApp

## O que é este projeto

Infográfico pessoal que visualiza o histórico de mensagens do WhatsApp entre Patrick e Camila.
Foi desenvolvido originalmente no Claude.ai e agora está sendo migrado para um projeto hospedável com URL pública.

**Objetivo desta migração:** nenhuma mudança visual ou funcional. O HTML final é a fonte da verdade. A única coisa que falta é uma forma de hospedar e acessar por URL pública.

---

## Arquivo de origem

O arquivo `infografico_final.html` na raiz deste projeto é o entregável completo e aprovado.
- É um HTML único, self-contained (sem dependências externas além de Google Fonts)
- Já é totalmente responsivo (mobile, tablet, desktop)
- Todos os dados estão embutidos como variáveis JS no final do arquivo
- **Não altere nada visualmente** — design, cores, tipografia, layout, textos e dados estão aprovados

---

## Stack e decisões técnicas

### Fontes
- **Fraunces** (serif, editorial) — headings, big numbers, citações
- **Inter** (sans-serif) — labels, dados, legendas
- Ambas via Google Fonts CDN

### Paleta Valentine
```
--bg:        #FBEFE7   (fundo creme rosado)
--cream:     #FFF6EE   (cards claros)
--pink:      #F4A8A0
--pink-deep: #E27A7A
--red:       #C73838
--red-deep:  #9B1F2E
--burgundy:  #5C1318   (cor principal de texto)
--gold:      #C89B4A   (destaques no heatmap)
--muted:     #8C5252
```

### Estrutura do HTML
O arquivo é dividido em 7 seções:
1. **Hero** — título "Patrick & Camila", datas, eyebrow
2. **Big Numbers** — grid 4×2 com métricas principais
3. **Como nos comunicamos pelos anos** — bar chart por ano
4. **Quando nos falamos** — heatmap dia × hora (scroll horizontal no mobile)
5. **Os emojis que dizem por nós** — pódio top 3 + lista top 15 com barras
6. **Nós dois, lado a lado** — comparison Patrick vs Camila
7. **A evolução do "te amo"** — timeline mensal + curiosidades

### Dados embutidos (JS no fim do arquivo)
Três variáveis injetadas pelo Python após análise do _chat.txt:
```js
const heatmapData = [...];  // matriz 7×24 (dia × hora)
const emojiData = [...];    // array de [emoji, count], top 15
const teAmoData = [...];    // array de [mes, count], fev/24 a mai/26
```

---

## Contexto dos dados

- **Chat analisado:** WhatsApp export de Patrick Farias e Camila Paiva
- **Período:** 16/02/2024 a 12/05/2026 (817 dias)
- **Total de mensagens:** 60.794
- **Script de análise original:** Python, arquivo `analyze.py` (pode não estar presente — os dados já estão embutidos no HTML)

---

## O que fazer nesta migração

### Tarefa única
Hospedar o `infografico_final.html` como uma página web acessível por URL pública.

### Abordagem recomendada
A solução mais simples é a correta. Opções em ordem de preferência:

1. **Next.js estático** — criar um projeto Next.js mínimo onde `infografico_final.html` é servido diretamente (via `public/` ou como página), fazer deploy na Vercel
2. **HTML puro na Vercel** — se Next.js for overhead desnecessário, um `vercel.json` + o HTML na raiz também resolve
3. **Qualquer outra solução** que resulte em URL pública estável

### O que NÃO fazer
- Não reescrever o HTML em JSX/React/componentes
- Não alterar CSS, cores, fontes ou layout
- Não mudar os dados embutidos
- Não adicionar features que não existiam (upload dinâmico, autenticação, etc.)
- Não usar frameworks pesados onde HTML simples resolve

---

## Estrutura esperada do projeto

```
/
├── CLAUDE.md                  ← este arquivo
├── infografico_final.html     ← o infográfico completo (não tocar)
└── [arquivos de deploy]       ← o mínimo necessário para hospedar
```

---

## Comandos úteis

```bash
# Se usar Next.js
npm run dev      # desenvolvimento local
npm run build    # build de produção
npx vercel       # deploy

# Se usar HTML puro com Vercel CLI
npx vercel       # deploy direto
```

---

## Notas de estilo e comportamento

- **Heatmap mobile:** tem scroll horizontal — é intencional, com hint "← arraste para o lado →"
- **Comparison (Patrick vs Camila):** empilhado no mobile, lado a lado no desktop
- **vs-center (coração ❤):** visível apenas no desktop, oculto no mobile
- **Breakpoints:**
  - Mobile pequeno: ≤ 380px
  - Mobile: ≤ 640px
  - Tablet: ≤ 900px
  - Desktop: > 900px

---

## Contato do projeto

Projeto pessoal de Patrick Farias. Não é produto público — é um presente/memória pessoal.
