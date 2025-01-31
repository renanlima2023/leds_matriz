# Contador de Números em Matriz de LEDs (5x5)

## Descrição
Este projeto define padrões de exibição numérica para uma matriz de LEDs 5x5, onde cada número de 0 a 9 é representado por uma matriz de valores booleanos (`true` para LED aceso e `false` para LED apagado). Ele pode ser utilizado para criar contadores ou displays numéricos em sistemas com matrizes de LEDs, utilizando a placa Raspberry Pi Pico e o protocolo WS2812.

## Estrutura do Projeto
O repositório contém os seguintes arquivos:

- **`count.h`**: Arquivo de cabeçalho que define os padrões numéricos em uma matriz 5x5.
- **`leds)matriz.c`**: Arquivo principal que contém a implementação para controlar os LEDs e o contador de números.
- **`ws2812.pio.h`**: Arquivo de cabeçalho que define o programa para controlar LEDs WS2812.
- **`pico/stdlib.h`**: Biblioteca para funcionalidades básicas do Raspberry Pi Pico.

## Como Funciona
O sistema usa uma matriz de LEDs 5x5 para exibir números de 0 a 9, com cada número sendo representado por um array booleano de tamanho 25 (5x5). O sistema também inclui dois botões para aumentar ou diminuir o contador e alternar entre os números.

- `1` indica um LED aceso.
- `0` indica um LED apagado.

Exemplo do padrão para o número "0":

```cpp
bool zero[NUM_PIXELS]  = { 1,1,1,1,1, 1,0,0,0,1, 1,0,0,0,1, 1,0,0,0,1, 1,1,1,1,1 };


## Funcionalidades

- O contador é incrementado ou decrementado ao pressionar os botões.
- A matriz de leds alterna entre os números com cores do arco-íris.
- Um LED vermelho pisca 5 vezes a cada 5 segundos para indicar o funcionamento correto.


## Requisitos
- Compilador C/C++
- Biblioteca para manipulação de LEDs WS2812 (caso utilize hardware físico, fornecido pela Bitdoglab)
- Raspberry Pi Pico


## Autor
Renan Lima

---
Se tiver alguma dúvida ou sugestão, fique à vontade para contribuir! 🚀

