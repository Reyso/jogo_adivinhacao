# Jogo de Adivinhação de Palavras Secretas

Este é um jogo simples de adivinhação de palavras secretas. O objetivo é adivinhar a palavra secreta a partir de tentativas feitas pelo usuário. A cada tentativa, o jogo irá fornecer feedback sobre as letras corretas, as posições corretas e as letras presentes, mas em posições erradas.

## Requisitos

- **Python 3.x**: O jogo foi desenvolvido em Python 3 e deve ser executado em qualquer sistema que tenha o Python 3 instalado.
- **Arquivos necessários**:
  - `tentativas.txt`: Um arquivo de texto contendo as tentativas feitas pelo jogador.

## Como Jogar

1. **Escolher uma palavra secreta**:
   - O jogo irá exibir uma lista de palavras secretas (com o número de letras de cada uma).
   - O jogador escolhe uma palavra secreta a partir da lista fornecida.

2. **Tentativas**:
   - O jogador deve escrever uma tentativa por vez no arquivo `tentativas.txt`.
   - Cada tentativa deve ser salva no arquivo, e depois o jogador deve rodar o jogo para obter o feedback.
   - **Somente uma tentativa por vez é permitida**. Após cada tentativa, o arquivo deve ser salvo, e o jogador deve rodar o jogo novamente. Se o jogador errar, ele pode repetir o processo com uma nova tentativa.
   - Para cada tentativa, o jogo informa quais letras estão corretas e em qual posição, ou se a letra está presente, mas em uma posição errada.

3. **Progresso**:
   - O progresso da tentativa será mostrado, com letras corretas reveladas nas posições corretas e as demais substituídas por underscores (`_`).

4. **Condição de Vitória**:
   - O jogo termina quando o jogador acerta a palavra secreta ou não consegue acertar após todas as tentativas.

## Funcionamento do Jogo

O jogo tem as seguintes etapas:

1. **Escolha de palavra secreta**: O jogador escolhe uma palavra secreta a partir de uma lista disponível no jogo.
2. **Carregamento das tentativas**: O jogo carrega as tentativas feitas pelo jogador a partir do arquivo `tentativas.txt`.
3. **Verificação das tentativas**: Para cada tentativa, o jogo verifica quais letras estão na posição correta e quais estão presentes, mas em posição errada.
4. **Progresso da palavra**: O jogo exibe o progresso da adivinhação em tempo real.

## Arquivos

- **tentativas.txt**: Contém as tentativas feitas pelo jogador. O jogador deve inserir uma tentativa por vez nesse arquivo, uma palavra por linha.
  - Exemplo de conteúdo:
    ```
    bash
    ```

## Funcionalidades e Regras

- **Ajuste de tamanho das tentativas**: As tentativas podem ter um número diferente de letras da palavra secreta, mas o jogo sempre ajusta o número de comparações ao tamanho da menor palavra.
- **Feedback de letras**: O jogo dá um feedback sobre as letras corretas e suas posições, além de informar se a letra está presente na palavra, mas na posição errada.
- **Progresso**: Após cada tentativa, o progresso é mostrado com underscores representando letras não adivinhadas.
- **Uma tentativa por vez**: O jogo permite apenas uma tentativa por vez. Após inserir uma palavra no arquivo `tentativas.txt`, o jogador deve salvar o arquivo e rodar o jogo para obter o feedback. Caso a tentativa esteja errada, o jogador deve repetir o processo com uma nova tentativa.

## Como Rodar o Jogo

1. Clone o repositório ou baixe os arquivos.
2. Coloque o arquivo `tentativas.txt` na mesma pasta do script.
3. Execute o script Python:

    ```bash
    python3 adivinhacao.py
    ```

4. Siga as instruções no terminal para escolher a palavra secreta e adivinhar as tentativas.

## Exemplo de Execução

Escolha uma das palavras secretas:

1- Palavra secreta com 6 letras
2- Palavra secreta com 4 letras
3- Palavra secreta com 5 letras

------------------------Digite o número da palavra secreta para iniciar o jogo: 1

A palavra chave tem 6 letras.

------------------------Tentativa: bash - Letras corretas nas posições: [1] A letra 'a' está na palavra secreta, mas na posição errada. Progresso: _ a _ _ _ _ ------------------------Tentativa: kernl - Letras corretas nas posições: [0] A letra 'k' está na palavra secreta, mas na posição errada. Progresso: k _ _ _ _ _ ------------------------Tentativa: byte - Nenhuma letra correta Progresso: _ _ _ _ _ ------------------------Parabéns! Você acertou a palavra secreta!
