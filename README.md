# EcoExploradores: Missão Reciclagem

Jogo educativo 2D desenvolvido com **Phaser 3.80.1**.

## Estrutura

```text
EcoExploradores-GitHub/
├── index.html          # Página principal
├── css/
│   └── style.css       # Estilos da página e do canvas
├── js/
│   └── game.js         # Código do jogo (cenas, regras, controles e áudio)
├── assets/
│   └── atlas.png       # Atlas de sprites e elementos visuais
├── .gitignore
└── README.md
```

## Como executar

A maneira recomendada é abrir a pasta com um servidor HTTP local. Por exemplo, com Python instalado:

```bash
python -m http.server 8000
```

Depois, acesse `http://localhost:8000` no navegador.

> **Importante:** nesta versão, o Phaser é carregado pelo CDN da cdnjs. Portanto, é necessária conexão com a internet para carregar a biblioteca. O atlas de imagens e os arquivos do jogo ficam locais. Para uma versão totalmente offline, será necessário incluir também o arquivo `phaser.min.js` localmente e ajustar a referência no `index.html`.

## Publicar no GitHub

1. Crie um repositório no GitHub.
2. Envie todos os arquivos e pastas desta estrutura (não apenas o `index.html`).
3. No repositório, abra **Settings → Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**.
5. Escolha a branch principal e a pasta `/ (root)`, depois salve.

O GitHub Pages publicará o `index.html` como página inicial.

## Controles

- **WASD / Setas:** movimentar
- **Espaço:** coletar
- **E:** conversar ou descartar
- **Q:** trocar item
- **I:** inventário
- **M:** mapa
- **N:** música
- **Esc:** pausar

O progresso é salvo no armazenamento local do navegador.
