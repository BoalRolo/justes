# Guia de Estilo: Portal da Aldeia (Justes)

## 1. Conceito Visual: "Moderno-Rústico"
O design deve equilibrar a tradição de uma aldeia de pedra com a clareza de uma interface moderna. 
- **Palavras-chave:** Minimalismo, Acolhedor, Terra, Legibilidade, Espaço.

## 2. Paleta de Cores (Tailwind Config)
- **Background (Fundo):** `#FDFBF7` (Um creme muito suave, cor de papel antigo/pedra clara).
- **Texto Principal:** `#2D2D2D` (Cinza Antracite, mais suave que o preto puro).
- **Cores de Destaque (Accent):**
  - **Primária:** `#4A5D4E` (Verde Floresta Seco - evoca a natureza e oliveiras).
  - **Secundária:** `#C17840` (Terracota/Barro - evoca telhados e terra).
- **Superfícies (Cards):** `#FFFFFF` (Branco puro para destacar do fundo creme).

## 3. Tipografia
- **Títulos (Headings):** 'Playfair Display' ou 'Source Serif 4' (Serifada). Deve transmitir elegância e peso histórico.
- **Corpo de Texto:** 'Geist' ou 'Inter' (Sans-serif). Focada em legibilidade moderna em ecrãs pequenos.

## 4. Elementos de Interface (UI)
- **Bordas:** Usar `rounded-2xl` para cards principais e fotos. Para botões, usar `rounded-lg`.
- **Sombras:** Usar `shadow-sm` ou sombras muito subtis. Evitar designs "pesados".
- **Botões:** Estilo retangular com cantos suaves (`rounded-lg`), cor de fundo Terracota (`#C17840`) e texto branco.
  - Transições suaves (`transition-all duration-300`).
  - Hover: Pequeno aumento de escala ou escurecimento da cor.

## 5. Fotografia
- As imagens devem ter cantos arredondados (`rounded-xl`).
- No Hero (topo do site), usar um overlay escuro de 30% para garantir que o texto branco seja legível por cima das fotos da aldeia.

## 6. Referências Visuais e Assets
- **Logótipo Principal:** Consultar `docs/assets/logo-justes.png`. Deve ser posicionado no canto superior esquerdo do Header, com uma altura máxima de 40px para manter a elegância.
    - **O que replicar (Crucial):** O Header minimalista com o logo "JUSTES" à esquerda. O Hero com a foto da aldeia e overlay escuro. A secção de Timeline com círculos claros para os anos. O estilo limpo dos cards de produtos e pontos de interesse.
- **Estrutura e Mood (Referência):** Ver `docs/assets/referencia-visual.png`.
  - **O que replicar:** O sistema de grelha (grid), o uso generoso de espaços em branco (whitespace), a forma como os cards de produtos são apresentados e a simplicidade da navegação.
  - **O que NÃO replicar:** As cores e o logótipo da referência. Usa a nossa paleta "Creme/Verde/Terracota".
- **Comportamento Responsivo:** No telemóvel, o logótipo deve manter-se visível e a navegação deve recolher para um "menu hambúrguer" simples.
