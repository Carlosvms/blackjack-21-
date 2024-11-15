# Blackjack em Java - Projeto acadêmico 🃏💻

### Descrição do Projeto
Este projeto é uma implementação de um jogo de **Blackjack** em Java, desenvolvido como atividade prática para uma disciplina de programação na faculdade. O jogo simula uma partida de Blackjack entre um jogador humano e o dealer (máquina) e foi projetado com foco na estruturação em pacotes e boas práticas de código.

### Funcionalidades
- Jogo de Blackjack básico entre o jogador e o dealer.
- Opções para o jogador: `comprar` (pedir carta) e `parar`.
- Dealer (máquina) segue as regras básicas de Blackjack, parando quando atinge um valor de 17 ou mais.
- Condições de vitória, derrota e empate, exibindo resultados claros ao final de cada rodada.

### Estrutura do Projeto

```plaintext
blackjack/
├── model/                  # Contém as classes de dados e lógica do jogo
│   ├── Carta.java           # Representa uma carta de baralho
│   ├── Baralho.java         # Gerencia o conjunto de cartas do jogo
│   ├── Mao.java             # Representa a mão de cartas de um jogador
├── controller/             # Contém a lógica do jogo
│   ├── JogoBlackjack.java   # Controla o fluxo de uma partida de Blackjack
├── view/            # Gerencia a interação com o jogador
│   ├── VisualizacaoConsole.java  # Interface do console para exibição de mensagens
└── main.java           # Classe principal para iniciar o jogo
```

### Estrutura das Classes

1. **model/**
   - **Carta**: Representa uma carta com seu naipe e valor.
   - **Baralho**: Um conjunto embaralhável de cartas para distribuir ao jogador e dealer.
   - **Mao**: Representa a mão de um jogador e calcula o valor total das cartas, ajustando o valor do Ás quando necessário.

2. **controller/**
   - **JogoBlackjack**: Classe principal do jogo, que gerencia o fluxo, interações e as regras do Blackjack.

3. **view/**
   - **VisualizacaoConsole**: Exibe mensagens e opções para o jogador no console.

4. **main.java**
   - Classe `main`: Ponto de entrada que inicializa o jogo.

### Como Executar

#### Pré-requisitos
- JDK 8 ou superior.

#### Compilação e Execução
1. Compile todos os arquivos Java:
   ```sh
   javac Principal.java model/*.java controller/*.java view/*.java
   ```
2. Execute o jogo:
   ```sh
   java main
   ```

### Regras Básicas
- **Objetivo**: Conseguir uma mão de cartas com valor total o mais próximo possível de 21, sem ultrapassá-lo.
- **Valores das Cartas**: Cartas numéricas valem seus números, figuras (valete, dama e rei) valem 10, e o Ás pode valer 1 ou 11.
- **Jogo**:
  - O jogador pode `comprar` para receber mais cartas ou `parar`  para finalizar a jogada.
  - O dealer compra cartas até alcançar 17 ou mais pontos.
  - Ganha quem estiver mais próximo de 21 sem ultrapassar.

### Exemplo de Execução

1. Ao iniciar o jogo, são distribuídas duas cartas para o jogador e duas para o dealer.
2. O jogador escolhe `comprar` para pedir mais uma carta ou `parar` para finalizar a jogada.
3. O dealer joga conforme as regras até alcançar um mínimo de 17 pontos.
4. O jogo exibe o resultado ao final, indicando o vencedor ou se houve empate.

### Autor
Projeto desenvolvido como parte das atividades acadêmicas da faculdade. 

