# Introdução à Programação de Computadores - Tema 2 - Super Trunfo em C: Desenvolvendo a Lógica do Jogo

# Super Trunfo - Nível Aventureiro

Este é um projeto em C desenvolvido como parte de um desafio da faculdade, nível "Aventureiro". O programa implementa uma versão interativa do jogo Super Trunfo, onde dois jogadores cadastram cartas representando países e competem com base em atributos escolhidos via menu.

## Descrição

O programa permite:
- Cadastrar duas cartas com informações de países (nome, população, área, PIB e pontos turísticos).
- Calcular automaticamente a densidade demográfica (população / área).
- Escolher um atributo para comparação através de um menu interativo.
- Comparar as cartas e exibir o resultado, incluindo os valores dos atributos e o vencedor.

### Atributos Disponíveis
1. **População** (int): Maior valor vence.
2. **Área** (float): Maior valor vence.
3. **PIB** (float): Maior valor vence.
4. **Pontos Turísticos** (int): Maior valor vence.
5. **Densidade Demográfica** (float): Menor valor vence.

## Pré-requisitos

- Compilador C (ex.: GCC).
- Sistema operacional compatível (Windows, Linux, macOS).

## Como Compilar

1. Clone o repositório:
```bash
 git clone https://github.com/Jonathanbez/LogicaProgramacao_SuperTrunfo_Estacio_CienciaComputacao.git
```
3. Navegue até o diretório:
```bash
   cd LogicaProgramacao_SuperTrunfo_Estacio_CienciaComputacao
```
3. Compile o código:
```bash
  gcc t2_na_da_strunfo.c -o t2_na_da_strunfo
```
Como Executar

Após compilar, execute o programa no terminal (No Linux ou macOS):
```bash
  ./t2_na_da_strunfo
```
No Windows:
```bash
  t2_na_da_strunfo.exe
```

O programa iniciará no terminal, solicitando o cadastro das cartas e, em seguida, a escolha do atributo para comparação.

## Exemplo de Uso

Aqui está um exemplo de como o programa funciona:
``` 
JOGO SUPER TRUNFO!
JOGADOR 1 - CADASTRE A CARTA

País: 
Brasil
População: 
203080756
Área: 
8510417.771
Digite o PIB: 
4101000000000
Quantidade de Pontos Turísticos: 
540

JOGADOR 2 - CADASTRE A CARTA

País: 
Canadá
População: 
38005238
Área: 
9984670
Digite o PIB: 
1808995000000
Quantidade de Pontos Turísticos: 
450
DADOS CARTA 1 - JOGADOR 1
JOGADOR 1 - País: Brasil
JOGADOR 1 - População: 203080756
JOGADOR 1 - Área: 8510418.00
JOGADOR 1 - PIB: 4100999872512.00
JOGADOR 1 - Pontos Turísticos: 540
JOGADOR 1 - Densidade demográfica: 23.862606
DADOS CARTA 2 - JOGADOR 2
JOGADOR 2 - País: Canadá
JOGADOR 2 - População: 38005238
JOGADOR 2 - Área: 9984670.00
JOGADOR 2 - PIB: 1808995057664.00
JOGADOR 2 - Pontos Turísticos: 450
JOGADOR 2 - Densidade demográfica: 3.806359

ESCOLHA DA COMPARAÇÃO
1. População
2. Área
3. PIB
4. Pontos Tuísticos
5. Densidade Demogŕafica
Digite a opção (1-5): 5
Comparação entre Densidade Demográfica: 
Pais 1: Brasil - Densidade Demográfica: 23.86
Pais 2: Canadá - Densidade Demográfica: 3.81
VENCEDOR: Canadá - JOGADOR 2
```
## Estrutura do Código

O código está organizado em seções principais:

- Cabeçalhos: Inclui <stdio.h>, <stdlib.h>, <time.h> (não usado neste nível) e <string.h> para manipulação de strings.
- Declaração de Variáveis: Define variáveis para armazenar os dados das cartas (nome, população, área, PIB, pontos turísticos e densidade).
- Entrada de Dados: Usa fgets() para ler o nome do país e scanf() para números, com getchar() para limpar o buffer de entrada.
- Exibição de Dados: Mostra os dados cadastrados de cada carta.
- Menu Interativo: Implementado com switch para selecionar o atributo de comparação.
- Lógica de Comparação: Usa if-else para determinar o vencedor com base no atributo escolhido, com regra especial para densidade demográfica.

# Autor

   Jonathan Bezerra - Estudante de Ciência da Computação na Estácio
   
   Linkedin - http://linkedin.com/in/jonathan-bezerra-b483b6148
  
# Licença

Este projeto é de uso educacional e não possui uma licença formal. Sinta-se à vontade para usá-lo como referência para estudos.

