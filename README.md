#  RPG Party Manager v2.0

> Um jogo de RPG baseado em texto desenvolvido em C com foco em gerenciamento de grupo (*Party*), combate dinâmico e manipulação de memória via Listas Encadeadas.

---

##  Demonstração

![Demonstração do RPG](caminho-ou-link-do-seu-gif.gif)

---

##  Sobre o Projeto

O **RPG Party Manager** é um sistema interativo em terminal onde o jogador atua como o líder de um grupo de aventureiros. O projeto foi desenvolvido como parte acadêmica pelas alunas **Geovanna Silva de Andrade** e **Keila Mouzinho Brandão**.

O sistema permite recrutar heróis com características e perícias aleatórias, gerenciar a equipe e explorar masmorras enfrentando encontros aleatórios (de *Ratos Gigantes* a *Tarrasques*!). 

###  Mecânica Principal: Permadeath
O jogo conta com a mecânica de **morte permanente**. Se os pontos de vida (HP) de um integrante da *party* chegarem a zero durante a batalha, ele morre e é removido da lista permanentemente!

---

##  Recursos e Funcionalidades

- **Recrutamento Dinâmico:** Crie heróis das classes *Guerreiro, Mago, Ladino, Paladino* ou *Clérigo*.
- **Gerenciamento de Perícias:** Sistema com 18 perícias (como *Atletismo*, *Arcanismo*, *Furtividade*, etc.) sorteadas aleatoriamente e opção de *reroll*.
- **Sistema de Combate e D20:** O encontro de monstros e a taxa de sucesso/dano utilizam mecânicas baseadas na rolagem de dados e nas perícias dos heróis.
- **Estrutura de Dados Eficiente:** Gerenciamento do grupo utilizando **Lista Encadeada Simples**, permitindo alocação e liberação de memória em tempo de execução (`malloc` e `free`).

---

##  Arquitetura do Código

O projeto está dividido de forma modular em três arquivos principais:

1. `rpg.h`: Interface do sistema com definição das estruturas (`TADs`), *enums*, protótipos de funções e comandos compatíveis com Windows/Linux.
2. `rpg.c`: Implementação de toda a lógica do jogo, cálculos de dano, funções utilitárias e manipulação de memória das listas.
3. `main.c`: Ponto de entrada do programa com o menu principal e a coordenação do fluxo da aplicação.

---

##  Como Executar o Projeto

### Pré-requisitos
* Compilador de linguagem C instalado (ex: `gcc`) **OU** ambiente de execução como o [OnlineGDB](https://www.onlinegdb.com/).

### Passo a Passo

1. Compile os arquivos C juntos:
   ```bash
   gcc main.c rpg.c -o rpg_game
