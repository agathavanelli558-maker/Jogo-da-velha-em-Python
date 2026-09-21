# Jogo da Velha

## Integrantes da Equipe

- Ágatha Do Prado Vanelli
- Lavínia Perina Ferraz

## Tema: Jogo da Velha

Um clássico **Jogo da Velha (Tic-Tac-Toe)** desenvolvido em **Python** para execução via terminal, contando com validações de jogadas, verificação automática de vitória e tratamento robusto de entradas inválidas.

## Como Jogar

| Entrada | Ação |
|---|---|
| `1` a `9` | Escolher a posição correspondente no tabuleiro para posicionar a peça |
| `Enter` | Confirmar a jogada selecionada |

## Objetivo

- Dois jogadores alternam turnos utilizando os símbolos **X** e **O**.
- O objetivo é alinhar três símbolos iguais em uma linha horizontal, vertical ou diagonal.
- O jogo termina com vitória para o jogador que completar a sequência ou com empate caso todas as posições sejam preenchidas sem um vencedor (**"deu velha"**).

## Pré-requisitos

Certifique-se de possuir o **Python** instalado em seu ambiente de execução.

## Executando

```bash
python "jogodavelha (1).py"
## Breve Descrição do Funcionamento do Sistema
```
O sistema executa um **loop interativo no terminal**. A cada rodada, o tabuleiro atual é exibido, o programa solicita a entrada numérica do jogador da vez, valida se a posição informada está livre e dentro do intervalo válido (1 a 9), atualiza o estado do jogo e verifica se houve vitória ou empate.

O fluxo alterna os turnos entre os jogadores **X** e **O** até o término da partida.

## Dicionário de Termos Técnicos

- **Terminal / CLI:** Interface de linha de comando utilizada para a interação textual entre o usuário e o programa.

- **Estrutura de Repetição (`while`):** Bloco de código que mantém o ciclo da partida ativo enquanto o número de jogadas for inferior ao limite máximo do tabuleiro.

- **Tratamento de Exceções (`try/except`):** Mecanismo de segurança para capturar erros de digitação, como inserção de letras ou caracteres especiais, impedindo o encerramento abrupto do programa.

- **Lista de Estados:** Estrutura de dados em Python que armazena os valores correntes de cada posição do tabuleiro, atualizando dinamicamente os símbolos dos jogadores.

## Estrutura do Código

O código é estruturado em **funções modulares** que dividem as responsabilidades do sistema.

### Funções Principais

- **`imprimir_tabuleiro(tabuleiro)`** — desenha e atualiza a representação visual do tabuleiro **3x3** no terminal.

- **`verificar_vitoria(tabuleiro, jogador)`** — percorre as combinações possíveis de vitória (**linhas, colunas e diagonais**) para determinar se o jogador atual completou uma sequência vencedora.

- **`jogo_da_velha()`** — gerencia o loop principal da partida, o controle de turnos entre os jogadores **X** e **O**, a validação de entradas e a verificação de empate técnico.

