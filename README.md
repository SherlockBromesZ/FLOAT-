# Funções de Arredondamento em C++: `floor()`, `ceil()`, `trunc()`, `round()` e `setprecision()`

Este documento explica as diferenças e usos das funções de arredondamento mais comuns em C++ para lidar com números de ponto flutuante.

## Introdução

Ao trabalhar com números de ponto flutuante, é importante entender como a precisão é tratada e como arredondar valores para diferentes propósitos. C++ oferece várias funções para lidar com isso:

* `floor(x)`
* `ceil(x)`
* `trunc(x)`
* `round(x)`
* `setprecision(n)`

## Descrição das Funções

### `floor(x)`

* **Objetivo:** Arredonda `x` para baixo para o inteiro mais próximo.
* **Exemplo:** `floor(2.8)` retorna `2`. `floor(-2.8)` retorna `-3`.
* **Uso comum:** Determinar o maior inteiro menor ou igual a um dado valor.

### `ceil(x)`

* **Objetivo:** Arredonda `x` para cima para o inteiro mais próximo.
* **Exemplo:** `ceil(2.8)` retorna `3`. `ceil(-2.8)` retorna `-2`.
* **Uso comum:** Determinar o menor inteiro maior ou igual a um dado valor.

### `trunc(x)`

* **Objetivo:** Trunca `x`, removendo todas as casas decimais.
* **Exemplo:** `trunc(2.8)` retorna `2`. `trunc(-2.8)` retorna `-2`.
* **Uso comum:** Descartar a parte fracionária de um número.

### `round(x)`

* **Objetivo:** Arredonda `x` para o inteiro mais próximo (para cima ou para baixo, dependendo de qual estiver mais perto).
* **Exemplo:** `round(2.8)` retorna `3`. `round(2.4)` retorna `2`. `round(-2.8)` retorna `-3`. 
* **Uso comum:** Arredondar para o inteiro mais próximo em geral.

### `setprecision(n)`

* **Objetivo:** Define a precisão da saída para `n` casas decimais quando usado com `fixed`.
* **Exemplo:** `cout << fixed << setprecision(2) << 3.14159;` exibe `3.14`.
* **Uso comum:** Controlar a exibição de números de ponto flutuante com um número específico de casas decimais.

## Tabela Resumo

| Função        | Descrição                                       | Exemplo (x = 2.8) | Exemplo (x = -2.8) |
|--------------|---------------------------------------------------|-------------------|--------------------|
| `floor(x)`   | Arredonda para baixo                              | 2                 | -3                 |
| `ceil(x)`    | Arredonda para cima                               | 3                 | -2                 |
| `trunc(x)`   | Remove casas decimais                             | 2                 | -2                 |
| `round(x)`   | Arredonda para o inteiro mais próximo            | 3                 | -3                 |
| `setprecision(n)` | Define a precisão da saída (com `fixed`) | 2.80 (n = 2)      | -2.80 (n = 2)      |

## Cabeçalhos Necessários

Para usar essas funções, inclua os seguintes cabeçalhos em seu código C++:

```cpp
#include <cmath>
#include <iomanip> 
