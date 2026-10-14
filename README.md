# Syntaxwear

Vitrine responsiva de tênis e sneakers, criada com HTML, CSS e JavaScript sem frameworks. O projeto apresenta categorias, destaques visuais, navegação responsiva e informações institucionais.

**Versão publicada:** [robsoncdesouza.github.io/ecommerce-syntaxwear](https://robsoncdesouza.github.io/ecommerce-syntaxwear/)

## Recursos

- Página inicial com banner de destaque e chamadas para ação.
- Seção de categorias: casual, esporte, moderno e futurista.
- Grade visual de produtos com imagens locais.
- Navbar horizontal em telas maiores e menu sanduíche em viewports de até 1359 px.
- Menu acessível por teclado, com suporte a Escape e fechamento ao clicar fora ou selecionar um link.
- Layout responsivo para tablet e celular.
- Rodapé com formulário visual de newsletter, links de navegação e ícones sociais em SVG.

## Tecnologias

- HTML5 semântico.
- CSS3, com estilos organizados por responsabilidade e media queries.
- JavaScript puro para controlar o menu responsivo.
- Fonte Ubuntu carregada do Google Fonts; é necessária conexão com a internet para buscar essa fonte. As fontes alternativas são definidas no CSS.

Não há dependências npm, processo de build ou etapa de compilação.

## Estrutura do projeto

```text
ecommerce-syntaxwear/
├── index.html
├── README.md
├── css/
│   ├── base.css
│   ├── layout.css
│   ├── reset.css
│   ├── responsive.css
│   ├── variables.css
│   └── components/
│       ├── footer.css
│       ├── header.css
│       ├── hero.css
│       ├── product-categories.css
│       └── product-grid.css
├── images/
│   ├── banner/
│   │   └── hero.jpg
│   ├── icons/
│   │   ├── bag.svg
│   │   ├── help.svg
│   │   └── user.svg
│   ├── logo/
│   │   └── logo.svg
│   └── products/
│       ├── card_imagem.jpg
│       ├── casual.jpg
│       ├── esporte.jpg
│       ├── futurista.jpg
│       ├── futurista-grid.jpg
│       ├── modelo-feminino.jpg
│       ├── moderno.jpg
│       ├── moderno-grid.jpg
│       ├── preto-azul-grid.jpg
│       └── roxo-verde-grid.jpg
└── js/
	└── navbar.js
```

## Como executar localmente

Como este é um site estático, você pode abrir `index.html` diretamente em um navegador. Para usar um servidor local, com Python 3 instalado, execute na pasta do projeto:

```bash
python -m http.server 8000
```

No Windows, também é possível usar o inicializador `py`:

```powershell
py -m http.server 8000
```

Depois, acesse [http://localhost:8000](http://localhost:8000).

## Organização dos estilos

- `reset.css`: normalização e regras globais de base.
- `variables.css`: fonte principal e variáveis CSS.
- `base.css`: tipografia e estilos gerais do documento.
- `components/`: estilos específicos para cabeçalho, banner, categorias, produtos e rodapé.
- `responsive.css`: adaptações por largura de viewport, carregadas depois dos estilos dos componentes.

O comportamento do menu está em `js/navbar.js`. Os links de navegação, os botões da vitrine, os links sociais e o formulário de newsletter ainda são elementos demonstrativos: não estão conectados a páginas, perfis, carrinho ou serviço de envio.

## Publicação

O projeto pode ser publicado em qualquer hospedagem de arquivos estáticos. A versão indicada neste repositório está disponível no GitHub Pages, no link no início deste documento.
