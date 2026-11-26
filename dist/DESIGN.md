# Swapp Design System — Extended

## Propósito

O Swapp Design System documenta a linguagem visual encontrada nos projetos originais e fornece arquivos reutilizáveis para desenvolvimento e ferramentas de IA. A documentação não é uma reformulação da marca: a fonte, cores, silhuetas e proporções originais são preservadas.

## Fontes consultadas

A base foi extraída dos projetos exportados do CodePen: Landing Page, Sign Up, User Profile, Settings, Credit Card Checkout, App Icon e 404 Page. O exemplo Calculator foi excluído da biblioteca visual de acordo com o escopo atual.

## Cores originais

| Token | Valor | Uso encontrado |
|---|---|---|
| `swapp-orange` | `#FF7B0D` | Ação e fundo principal em botões e gradientes |
| `swapp-orange-light` | `#FFA84C` | Ponta clara do gradiente e hover do botão laranja |
| `swapp-orange-top` | `#FF7F13` | Barra superior dos layouts mobile |
| `swapp-orange-border` | `#FFA200` | Borda dos campos de texto |
| `swapp-magenta` | `#C40BD5` | Botão principal e fundo do fluxo 404 |
| `swapp-magenta-hover` | `#EA00FF` | Hover do botão magenta e gradiente 404 |
| `swapp-facebook` | `#3A589A` | Botão de cadastro social |
| `swapp-facebook-hover` | `#4E6DB2` | Hover do botão social |
| `swapp-coral` | `#E19C8A` | Texto de campo e teclas circulares |
| `swapp-placeholder` | `#E1E1E1` | Texto de placeholder |
| `swapp-orange-profile` | `#FFA446` | Fundo de linhas de perfil |
| `swapp-orange-hero` | `#FF8820` | Sobreposição da hero da landing page |
| `swapp-white` | `#FFFFFF` | Texto e superfícies de componentes |
| `swapp-disabled-gray` | `#CCCCCC` | Fundo do switch desativado |

### Gradientes originais
- Superfícies e app icon: `linear-gradient(135deg, #FFA84C 0%, #FF7B0D 100%)`.
- 404: `linear-gradient(135deg, #C40BD5 0%, #EA00FF 100%)`.
- Landing hero possui sobreposição `#FF8820`; a barra superior dos fluxos mobile usa `#FF7F13`.

## Tipografia original

`Averia Sans Libre` é a única família encontrada nos CSS enviados. Os botões e inputs usam 15px; o body usa 14px na maioria dos fluxos mobile. O peso não foi padronizado de forma explícita nos fontes, portanto não se impõe uma escala de pesos inexistente.

## Dimensões e forma observadas
- Mockup mobile: 270 × 480px; raio de 8px.
- Botões: altura de 44px, raio de 50px; no Sign Up e checkout, largura inicial de 200px e hover 220px. Na página 404, a largura declarada é 250px e hover 270px.
- Campos: largura declarada de 170px, conteúdo de 24px mais padding vertical de 10px, borda de 1px e raio de 50px. Campo de cartão: largura de 122px.
- Perfil: imagem circular de 90px.
- Barra superior de mobile: 50px de altura.
- Switch Settings: trilho de 40 × 18px e knob de 14px.
- Sombra do mockup: `10px 25px 60px 10px rgba(0,0,0,0.2)`.

## Componentes documentados

### Botão principal
- Origem: Sign Up e Credit Card Checkout.
- Padrão: magenta `#C40BD5`, hover `#EA00FF`, 44px de altura, raio de 50px, Averia Sans Libre 15px, caixa alta.
- Recomendação: foco visível, disabled/loading, largura fluida em mobile, feedback de envio.

### Botão laranja
- Origem: Landing Page e 404 Page.
- Padrão: laranja `#FF7B0D`, hover `#FFA84C`, 44px, raio 50px. Largura varia por projeto.
- Recomendação: reservar para ações de marca e contexto; não confundir automaticamente com CTA transacional magenta.

### Login social
- Origem: Sign Up.
- Padrão: azul `#3A589A`, hover `#4E6DB2`, 50px, cantos inferiores de 8px no layout original.

### Campo de texto e senha
- Origem: Sign Up e Credit Card Checkout.
- Padrão: borda `#FFA200`, raio 50px, fonte 15px, texto `#E19C8A`, placeholder `#E1E1E1`.
- Recomendação: rótulo persistente, validação, helper text, erro associado por `aria-describedby`, foco visível e disabled.

### Campo de cartão
- Origem: Credit Card Checkout.
- Padrão: largura declarada de 122px, mesma linguagem de borda e raio do campo comum.
- Recomendação: agrupar número, validade e código de segurança com labels e máscara apropriada.

### Linhas de configuração
- Origem: Settings e User Profile.
- Padrão: linha laranja, texto branco, ícone branco; badge branco com texto coral `#E19C8A`.
- Recomendação: estado clicável, foco, separadores consistentes e estado disabled explícito.

### Switch
- Origem: Settings.
- Padrão observado: trilho 40×18px, knob 14px; estado ativo com superfície branca e knob laranja `#FF7F13`.
- Recomendação: usar input nativo acessível, texto de estado e foco visível.

### Perfil e indicadores
- Origem: User Profile.
- Padrão: foto circular 90px, nome 24px, linhas laranja `#FFA446`, mini ações circulares magenta.
- Recomendação: fallback de avatar, truncamento de nome e contagem com unidade explícita.

### Badge
- Origem: Settings e User Profile.
- Padrão: fundo branco, texto coral, formato pill.

### Ícones
- Biblioteca incluída: 42 ícones SVG, 24×24, traço consistente. Cada arquivo individual pode ser copiado ou importado.
- Não substitua o logotipo pela seta de troca ou por qualquer ícone da biblioteca.

## Logotipo oficial

O arquivo-mestre é `assets/swapp-logo.png`, fornecido pelo projeto e usado diretamente no portal. Preserve sua proporção original e a transparência; nunca aplique crop, máscara, fundo branco ou ícone substituto. `assets/swapp-logo.svg` é uma vetorização auxiliar do contorno extraído do PNG e só deve ser usada quando um formato vetorial for necessário. O PNG continua sendo a referência visual oficial.

## Acessibilidade e evolução proposta

As regras de acessibilidade aqui são recomendações de evolução, não características garantidas nos protótipos históricos: foco visível, labels, contraste verificado em contexto, mensagens de erro associadas a campos, estados disabled/loading e alvos de toque apropriados.

## Uso por ferramentas de IA

Inclua este documento em `AGENTS.md` ou `CLAUDE.md`, ou referencie-o nas rules do Cursor. Para contexto curto, use `DESIGN.compact.md`. Para configurar estilo, importe `variables.css` ou a entrada `tailwind.css`; para pipelines de design tokens, consuma `tokens.json`.

## Downloads

Os arquivos de distribuição ficam em `dist/`. O pacote consolidado `swapp-ai-kit.zip` reúne documentos, tokens, tema Tailwind e ícones.