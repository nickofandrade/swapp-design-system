# Swapp Design System

Portal de documentação e distribuição do Swapp, com arquitetura inspirada no Hubble da Kenlo: navegação lateral, prévia renderizada e painel técnico com abas, Compact/Extended, copiar e baixar. Em telas compactas, o usuário alterna entre Prévia e Documentação sem comprimir os dois painéis.

## Portal
Abra `index.html` em hospedagem estática. Não há etapa de build. GitHub Pages publica a raiz do branch `main`.

## Arquivos para desenvolvimento e IA
- `dist/DESIGN.md`: especificação completa para agentes e desenvolvedores.
- `dist/DESIGN.compact.md`: contexto compacto.
- `dist/tailwind.css`: tema para Tailwind CSS v4.
- `dist/variables.css`: CSS variables e padrões reutilizáveis.
- `dist/tokens.json`: tokens no formato W3C DTCG.
- `dist/icons/`: 42 SVGs individuais.
- `AGENTS.md`, `CLAUDE.md`, `.cursor/rules/swapp-design.mdc`: instruções de entrada para diferentes agentes.
- `swapp-ai-kit.zip`: bundle compacto com documentação, tokens, estilos, ícones e marca.
- `reference-source/original-exports.zip`: exports originais dos sete projetos usados como fonte.

## Fonte e rastreabilidade
A biblioteca foi estruturada a partir dos CSS e HTML exportados do CodePen: Landing Page, Sign Up, User Profile, Settings, Credit Card Checkout, App Icon e 404 Page. A calculadora não é apresentada como tela ou exemplo nesta biblioteca. Valores observados nos arquivos originais são identificados como origem; escalas, acessibilidade e consistência são rotuladas como evolução proposta.

## Marca
`assets/swapp-logo.png` é o arquivo-mestre original fornecido. O portal o utiliza diretamente, sem recorte, redesenho ou alteração de proporção. `assets/swapp-logo.svg` é uma vetorização auxiliar do contorno e não substitui o PNG original.