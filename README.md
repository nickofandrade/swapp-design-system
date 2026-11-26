# Swapp Design System

Biblioteca de referência com estrutura inspirada no Hubble Design System da Kenlo: prévia renderizada à esquerda e documentação/distribuição à direita.

## Começar
Abra `index.html` em um servidor estático. Não há build step. O site é compatível com GitHub Pages na raiz do branch `main`.

## Distribuição para código e IA
- `dist/DESIGN.md`: documentação extended para contexto de agentes.
- `dist/DESIGN.compact.md`: instruções compactas.
- `dist/tailwind.css`: entrada de tema para Tailwind CSS v4.
- `dist/variables.css`: CSS variables e padrões reutilizáveis.
- `dist/tokens.json`: tokens W3C DTCG.
- 42 ícones SVG individuais dentro de `dist/icons/` no pacote `swapp-ai-kit.zip`.
- `swapp-ai-kit.zip`: bundle com docs, tokens, styles, ícones e marca.
- `AGENTS.md`, `CLAUDE.md`, `.cursor/rules/swapp-design.mdc`: pontos de entrada para agentes.

## Base e rastreabilidade
Os tokens foram extraídos dos CSS dos projetos exportados do CodePen: Landing Page, Sign Up, User Profile, Settings, Credit Card Checkout, App Icon e 404 Page. A calculadora não aparece na biblioteca nem nos exemplos de telas, conforme escopo definido. Valores e componentes identificados como originais vêm dos arquivos fonte; recomendações de acessibilidade e consistência estão rotuladas como evolução proposta.

## Marca
O logotipo original é mantido em `assets/swapp-logo.svg`, com contorno vetorizado a partir do arquivo mestre e fundo transparente. O PNG mestre original é incluído no pacote `swapp-ai-kit.zip`.