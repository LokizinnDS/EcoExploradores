# EcoExploradores: Missão Reciclagem

Jogo educativo 2D desenvolvido como projeto-piloto para apresentar, de forma interativa, conceitos de coleta seletiva, reciclagem e cuidado com o meio ambiente. A tela inicial identifica o projeto como **EcoExploradores: Missão Reciclagem · SENAI Campo Mourão**.

## Objetivo

Explore os ambientes, converse com personagens, recolha resíduos espalhados pelo mapa e descarte cada material na lixeira correspondente. Os descartes corretos e os desafios rendem pontos e ajudam a avançar nas missões até alcançar a classificação **Guardião Ambiental**.

## Como jogar

1. Na tela inicial, selecione **Jogar** para iniciar uma partida ou **Continuar** para carregar um progresso salvo, quando disponível.
2. Explore as regiões e aproxime-se dos resíduos para coletá-los.
3. Converse com moradores, educadores e outros personagens para receber orientações e responder perguntas.
4. Leve os materiais até as lixeiras e faça o descarte correto.
5. Complete as cinco missões para concluir a jornada.

### Controles

| Tecla | Ação |
|---|---|
| `W`, `A`, `S`, `D` ou setas | Movimentar o personagem |
| `ESPAÇO` | Coletar um resíduo próximo |
| `E` | Conversar ou descartar o item selecionado na lixeira próxima |
| `Q` | Alternar o item selecionado no inventário |
| `I` | Abrir/fechar o inventário |
| `M` | Abrir/fechar o mapa |
| `N` | Ligar/desligar a música |
| `ESC` | Pausar/retomar o jogo |
| `1`, `2` ou `3` | Escolher uma resposta nos questionários |

O inventário comporta até **15 itens**. Se estiver cheio, descarte materiais antes de continuar coletando.

## Separação dos resíduos

O jogo apresenta seis categorias:

| Cor da lixeira | Categoria |
|---|---|
| Azul | Papel |
| Vermelha | Plástico |
| Verde | Vidro |
| Amarela | Metal |
| Marrom | Orgânico |
| Cinza | Rejeitos |

Os materiais possuem orientações educativas. Descartar na categoria correta soma pontos; usar uma lixeira incorreta gera uma penalidade e uma mensagem explicativa.

## Regiões exploráveis

O mapa contém sete regiões conectadas:

- **Praça Central:** ponto inicial, apresentação do projeto e orientações sobre coleta seletiva.
- **Parque Ecológico:** biodiversidade, limpeza de áreas verdes e impactos do lixo na natureza.
- **Bairro Urbano:** casas, comércio, moradores e separação de resíduos.
- **Área Tecnológica SENAI:** espaço de aprendizagem e desafio com o instrutor.
- **Centro Comercial:** comércio, escola, serviços e circulação urbana.
- **Floresta Preservada:** biodiversidade, água e proteção dos animais.
- **Vila Residencial:** hábitos sustentáveis e descarte doméstico.

As regiões são reveladas no mapa conforme o jogador as visita.

## Missões

1. **Primeiros Passos:** conversar com a ambientalista e realizar 5 descartes corretos.
2. **Parque Limpo:** visitar o parque e alcançar 15 descartes corretos.
3. **Bairro Sustentável:** visitar o bairro e alcançar 30 descartes corretos.
4. **Tecnologia Verde:** visitar a área SENAI e concluir o desafio do instrutor.
5. **Guardião Ambiental:** alcançar 40 descartes corretos.

### Pontuação

- Coletar um resíduo: **+5 pontos**.
- Descartar corretamente: **+10 pontos**.
- Responder corretamente a um questionário: **+20 pontos**.
- Concluir uma missão: **+100 pontos**.
- Descartar na lixeira errada: **−5 pontos**.

As classificações são: Iniciante Ambiental, Coletor Consciente, Protetor da Natureza, Especialista em Reciclagem e Guardião Ambiental.

## Como executar

### Usando o Visual Studio Code

1. Baixe ou clone este repositório.
2. Abra a pasta do projeto no Visual Studio Code.
3. Inicie um servidor local, por exemplo, com a extensão **Live Server**.
4. Abra o endereço local informado pelo servidor.

### Usando Python

Com Python instalado, abra o terminal na pasta do projeto e execute:

```bash
python -m http.server 8000
```

Acesse `http://localhost:8000` no navegador.

O projeto também pode ser publicado pelo **GitHub Pages**, mantendo a estrutura de pastas e arquivos.

## Tecnologias utilizadas

- **HTML5:** estrutura da página.
- **CSS:** apresentação da tela.
- **JavaScript:** lógica do jogo, movimentação, inventário, missões, diálogos e salvamento.
- **Phaser 3.80.1:** engine 2D, cenas, animações e física.
- **PNG atlas:** sprites do personagem, NPCs, cenários, resíduos, lixeiras e efeitos.
- **Web Audio API:** geração de efeitos sonoros e notas musicais.
- **localStorage:** armazenamento do progresso no navegador.

## Estrutura do projeto

```text
EcoExploradores-GitHub/
├── index.html
├── css/
│   └── style.css
├── js/
│   └── game.js
├── assets/
│   └── atlas.png
├── README.md
├── .gitignore
└── original-jogo.html
```

## Salvamento do progresso

O progresso é armazenado no `localStorage` do navegador. Portanto, a opção **Continuar** funciona no mesmo navegador e dispositivo em que a partida foi salva. Limpar os dados do navegador pode apagar esse progresso.

## Observações importantes

- **Internet:** nesta versão, a biblioteca Phaser 3.80.1 é carregada por CDN no `index.html`. Assim, é necessária conexão com a internet para carregar essa biblioteca. Apesar de os arquivos do jogo estarem na pasta do projeto, esta versão ainda não é totalmente offline.
- **Coleta de Campo Mourão:** existe no código um painel preparado para apresentar dias e bairros da coleta, mas a lista `COLETA` está vazia nesta versão. Os horários e bairros oficiais ainda precisam ser cadastrados e conferidos com a Prefeitura antes de serem apresentados como calendário real.
- **Projeto-piloto:** mapas, textos, missões e conteúdos podem ser ajustados conforme os testes com os visitantes.

## Publicação no GitHub Pages

1. Crie um repositório no GitHub.
2. Envie todos os arquivos e pastas, preservando a estrutura apresentada acima.
3. Nas configurações do repositório, abra **Pages**.
4. Escolha a branch principal (`main`) e a pasta raiz (`/root`).
5. Salve e aguarde a publicação do endereço do jogo.

---

**EcoExploradores: Missão Reciclagem** — aprender a separar resíduos explorando, conversando e jogando.
