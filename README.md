# SnakePy - Projeto IP

PT-BR | [English](#english)

Jogo da cobrinha feito em Python com Pygame, com sistema de pontuacao por tipo de comida e obstaculo de bomba.

## PT-BR

### Funcionalidades

- Movimento da cobra com as setas do teclado.
- Comidas com 3 tipos (verde, azul e amarela), cada uma com valor de pontos diferente.
- Bomba gerada em posicao aleatoria (evitando cobra e comida).
- Tela de fim de jogo com pontuacao total, capturas por tipo de comida e opcao de reiniciar.

### Requisitos

- Python 3.10+ (recomendado)
- Pygame

### Instalacao

1. Crie e ative um ambiente virtual (opcional, mas recomendado).
2. Instale a dependencia:

```bash
pip install pygame
```

### Como executar

Na pasta raiz do projeto, rode:

```bash
python main_py
```

### Controles

- Seta para cima: mover para cima
- Seta para baixo: mover para baixo
- Seta para esquerda: mover para esquerda
- Seta para direita: mover para direita
- Enter: iniciar no menu e reiniciar apos game over

### Pontuacao

- Comida verde: +1 ponto
- Comida azul: +2 pontos
- Comida amarela: +3 pontos

### Estrutura principal

- `main_py`: loop principal do jogo e menu.
- `settings.py`: configuracoes gerais (tela, cores, clock e carregamento de sprites).
- `sprites.py`: classe de comida (`Comida`) e logica de spawn/animacao.
- `functions.py`: funcoes auxiliares (movimento, desenho, bomba e fim de jogo).

O repositorio tambem contem pastas/arquivos de versoes intermediarias e correcoes, como historico de desenvolvimento.

### Observacoes importantes

- O arquivo `settings.py` espera pastas de assets na raiz.
- Pasta `imagens/`: precisa conter `comida1.png`, `comida2.png` e `comida3.png`.
- Pasta `sons/`: reservada para uso de audio.
- Se essas pastas nao estiverem presentes, o jogo nao iniciara corretamente.

### Possiveis melhorias

- Salvar recorde em arquivo local.
- Adicionar niveis de dificuldade.
- Inserir trilha sonora e efeitos.
- Organizar snapshots/historico em pasta separada (`docs/` ou `historico/`).

---

## English

Snake game built with Python and Pygame, featuring score by food type and a bomb obstacle.

### Features

- Snake movement using keyboard arrow keys.
- 3 food types (green, blue, yellow), each with different score values.
- Bomb generated at a random position (avoids snake and food).
- Game over screen with total score, captures per food type, and restart option.

### Requirements

- Python 3.10+ (recommended)
- Pygame

### Installation

1. Create and activate a virtual environment (optional but recommended).
2. Install dependency:

```bash
pip install pygame
```

### Run

From the project root folder, run:

```bash
python main_py
```

### Controls

- Up arrow: move up
- Down arrow: move down
- Left arrow: move left
- Right arrow: move right
- Enter: start from menu and restart after game over

### Scoring

- Green food: +1 point
- Blue food: +2 points
- Yellow food: +3 points

### Main structure

- `main_py`: main game loop and menu.
- `settings.py`: general settings (screen, colors, clock, and sprite loading).
- `sprites.py`: food class (`Comida`) and spawn/animation logic.
- `functions.py`: helper functions (movement, rendering, bomb, and game over).

The repository also includes intermediate/fix versions as development history.

### Important notes

- `settings.py` expects asset folders at the project root.
- Folder `imagens/`: must contain `comida1.png`, `comida2.png`, and `comida3.png`.
- Folder `sons/`: reserved for audio usage.
- If these folders are missing, the game will not start correctly.

### Possible improvements

- Save high score locally.
- Add difficulty levels.
- Add soundtrack and sound effects.
- Organize snapshots/history into a dedicated folder (`docs/` or `historico/`).