# Swapp Design System — Compact

Use este documento como contexto curto ao gerar ou modificar interfaces do Swapp. Preserve a marca e os padrões abaixo; prefira reutilizar os componentes existentes em vez de criar variações sem necessidade.

## Identidade visual original
- Fonte de interface: `Averia Sans Libre`, cursive.
- Laranja principal: `#FF7B0D`; laranja claro: `#FFA84C`; laranja superior: `#FF7F13`; borda de campo: `#FFA200`.
- Magenta: `#C40BD5`; hover magenta: `#EA00FF`.
- Social: `#3A589A`; hover social: `#4E6DB2`.
- Coral: `#E19C8A`; placeholder: `#E1E1E1`; branco: `#FFFFFF`.
- Botões principais originais: 44px de altura, raio 50px, Averia Sans Libre 15px, caixa alta. Magenta nos fluxos de cadastro/checkout; laranja em ações de marca e 404.
- Campos originais: raio 50px, borda `#FFA200`, texto `#E19C8A`, placeholder `#E1E1E1`, fonte 15px. Largura de referência: 170px (campos text/password); checkout também usa campo de cartão de 122px.
- Mockup mobile original: 270 × 480px, raio 8px. Barra superior: 50px, `#FF7F13`.
- Cadastro social: azul `#3A589A`, hover `#4E6DB2`, faixa de 50px.
- Perfil: foto circular de 90px; ações circulares magenta.
- Settings: linhas de 40px de switch com trilho cinza e acento laranja; badge branco com texto coral.
- Tela 404: gradiente `#C40BD5` → `#EA00FF`.

## Regras para geração de UI
1. Não redesenhe, substitua, simplifique ou invente o logo. Use `assets/swapp-logo.png` como arquivo-mestre. Preserve a proporção e a transparência; `assets/swapp-logo.svg` é apenas uma vetorização auxiliar do contorno, não substitui o PNG original.
2. Use `Averia Sans Libre` para UI. Não substitua a família sem solicitação explícita.
3. Preserve a combinação laranja + magenta e o azul reservado ao login social. Não transforme o projeto em outro sistema visual.
4. Preserve a linguagem arredondada dos botões e campos. Evite cantos quadrados nos CTAs e inputs.
5. Separe o que é padrão histórico do que é evolução. Não atribua ao produto uma regra que não esteja nos fontes.
6. Componentes acessíveis devem ter foco visível, rótulos persistentes, estados disabled/error/loading e alvos de toque adequados; isso é recomendação de evolução.
7. Use os SVG em `dist/icons/` e mantenha traço consistente; prefira ícones 24×24.
8. Não inclua a calculadora nos exemplos de telas ou na navegação desta biblioteca.

## Arquivos
- `dist/variables.css`: CSS variables e padrões de componentes.
- `dist/tailwind.css`: entrada de tema para Tailwind CSS v4.
- `dist/tokens.json`: tokens no formato W3C DTCG.
- 42 ícones SVG individuais, incluídos em `swapp-ai-kit.zip` dentro de `dist/icons/`.
- `assets/swapp-logo.png`: arquivo-mestre original da marca.
- `assets/swapp-logo.svg`: vetorização auxiliar do contorno, opcional.


## App icon
Use `assets/swapp-app-icon.svg` ou `.png`: inicial S extraída do logotipo original sobre o gradiente laranja. Não substitua por uma letra tipográfica genérica.