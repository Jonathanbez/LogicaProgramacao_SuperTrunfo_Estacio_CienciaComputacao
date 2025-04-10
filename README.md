# Introdução à Programação de Computadores - Tema 2 - Super Trunfo em C: Desenvolvendo a Lógica do Jogo

# Super Trunfo - Nível Aventureiro

Este é um projeto em C desenvolvido como parte de um exercicio da faculdade Estácio graduacao em Ciência da Computação, nível "Mestre". O programa implementa uma versão interativa do jogo Super Trunfo, onde dois jogadores cadastram cartas representando países e competem com base em atributos escolhidos via menu.

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

## Regras
- **População, Área, PIB, Pontos Turísticos:** Maior valor ganha 1 ponto.
- **Densidade Demográfica:** Menor valor ganha 1 ponto.
- Empates não dão pontos.

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
  gcc t2_nm_da_strunfo.c -o t2_nm_da_strunfo
```
Como Executar

Após compilar, execute o programa no terminal (No Linux ou macOS):
```bash
  ./t2_nm_da_strunfo
```
No Windows:
```bash
  t2_nm_da_strunfo.exe
```

O programa iniciará no terminal, solicitando o cadastro das cartas e, em seguida, a escolha do atributo para comparação.

## Como Usar
1. Cadastre a carta do Jogador 1 (País, População, Área, PIB, Pontos Turísticos).
2. Cadastre a carta do Jogador 2.
3. Escolha:
   - `A`: Comparar 2 atributos (digite dois números de 1 a 5).
   - `B`: Comparar todos os atributos.
4. Veja o resultado com os pontos e o vencedor.

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
8510418
Digite o PIB: 
2130000000000
Quantidade de Pontos Turísticos: 
500

JOGADOR 2 - CADASTRE A CARTA

País: 
Canadá
População: 
41528680
Área: 
9984670
Digite o PIB: 
2140000000000
Quantidade de Pontos Turísticos: 
400

*** ESCOLHA DA COMPARAÇÃO ***
A. Escolha 2 atributos
B. Escolha todos os atributos
Digite o tipo de comparação (A ou B): 
A

*** Escolha quais atributos das cartas para comparação ***
1. População
2. Área
3. PIB
4. Pontos Turísticos
5. Densidade Demográfica
Escolha o primeiro atributo(1-5): 5
Escolha o segundo atributo(1-5): 4

OUTPUT:
DADOS CARTA 1 - JOGADOR 1
JOGADOR 1 - País: Brasil
JOGADOR 1 - População: 203080756
JOGADOR 1 - Área: 8510418.00
JOGADOR 1 - PIB: 2130000000000.00
JOGADOR 1 - Pontos Turísticos: 500
JOGADOR 1 - Densidade demográfica: 23.862606

DADOS CARTA 2 - JOGADOR 2
JOGADOR 2 - País: Canadá
JOGADOR 2 - População: 41528680
JOGADOR 2 - Área: 9984670.00
JOGADOR 2 - PIB: 2140000000000.00
JOGADOR 2 - Pontos Turísticos: 400
JOGADOR 2 - Densidade demográfica: 4.159244

Densidade - Jogador 1: 23.86 vs Jogador 2: 4.16
Pontos Turísticos - Jogador 1: 500 vs Jogador 2: 400

RESULTADO:
Jogador 1: 1 pontos
Jogador 2: 1 pontos
Vencedor: Empate
```

## Estrutura do Código

O código está organizado em seções principais:

- **Cabeçalhos:** Inclui `<stdio.h>` para entrada/saída, `<stdlib.h>` para funções padrão e `<string.h>` para manipulação de strings.
- **Declaração de Variáveis:** Define variáveis para os dados das cartas (nome do país como string, população e pontos turísticos como inteiros, área e PIB como floats, densidade calculada como float) e controle do jogo (opção, atributos escolhidos, somas de pontos).
- **Entrada de Dados:** Usa `fgets()` para ler o nome do país e `scanf()` para números, com `getchar()` para limpar o buffer após entradas numéricas.
- **Cálculo da Densidade:** Calcula a densidade demográfica dividindo população por área para cada carta.
- **Exibição de Dados:** Mostra os dados cadastrados de cada carta com formatação específica (ex.: %.2f para floats).
- **Menu Interativo:** Usa `switch` para escolher entre comparar 2 atributos (opção A) ou todos (opção B), com sub-`switch` para selecionar atributos na opção A.
- **Lógica de Comparação:** Emprega operadores ternários (`?:`) para atribuir pontos (1 ou 0) com base em comparações, com regra especial para densidade (menor vence), e `if-else` para verificar atributos duplicados na opção A.

## Autor

Jonathan Bezerra - Estudante de Ciência da Computação na Estácio

LinkedIn - [http://linkedin.com/in/jonathan-bezerra-b483b6148](http://linkedin.com/in/jonathan-bezerra-b483b6148)

## Licença

Este projeto é de uso educacional e não possui uma licença formal. Sinta-se à vontade para usá-lo como referência para estudos.

