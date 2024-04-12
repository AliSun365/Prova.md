# PROVA :pencil: 

### Exercício 01: Solucione o erro

```c 
// Corrija o seguinte código para que ele imprima números impares menores que 10

#include <stdio.h>

int main()
{
  for (int i = 0; i < 10; i++)
  {
    if(/* condição para verificar se 'i' é impar*/)
    {
       printf("%d\n", i);
    }

  }
  return 0;
}
```
### Exercício 02: Determinar o maior 
Escreva um programa que receba três números e determina qual é o maior.

### Exercício 03: Palíndromos
Palíndromos são números que têm o mesmo valor se lidos da esquerda para a direita
ou da direita para a esquerda. Exemplos: 44, 232, etc. Faça um programa que determine
e escreva todos os números inteiros entre 1000 que 10000 que são palíndromos.

### Exercício 04: Árvore
Faça um programa que imprima uma árvore de Natal, considerando uma altura
especificada pelo usuário. Para h=3:
```
  I
 *I*
**I**
```

### Exercício 05: Corriga o código 

```c 
// Corrija o seguinte código para que ele imprima números impares menores que 10

#include <stdio.h>

int main()
{
  int i,j;

  // Erro 1: Loop infinito
  for (i = 0; i < 5; i--)
  {
    printf("i = %d\n", i);
  }

  // Erro 2: Condição de loop incorreta
  for (j = 0; j < 5; j += 2)
  {
    printf("j = %d\n", j);
  }

  // Lógica de verificação de número primo incorreta
  int num = 9, primo = 1;
  for (i = 2; i < num; i++)
  {
    if (num % i == 0)
    {
      primo = 0;
    }
  }

  if(primo = 1)
  {
    printf("%d é um número primo.\n", num);
  } else {
     printf("%d não é um número primo.\n", num);
  }

  return 0;
}
```
### Exercício 06: Média
Escreva um programa que leia 10 números e computa a média, máximo e menor valor.

### Exercício 07: Corrigir erro 
Aqui está outro exemplo de programa em C que contém um erro lógico para você identificar e corrigir
 ```c 
// Corrija o seguinte código para que ele imprima números impares menores que 10

#include <stdio.h>

int main()
{
  int num, soma = 0;

  // O objetivo é somar números pares menores que 10
  for (num = 1; num < 10; num++)
  {
    if(num % 2 = 0)
    {
       soma += num;
    }
  }

   printf("A soma dos números pares menores que 10 é: %d\n", soma);

  return 0;
}
```

### Exercício 08: Cálculo salário 
Implemente um programa para uma revendedora de carros que calcule o salário de
cada vendedor. Considere que todos os carros têm o mesmo valor, e que a revendedora
paga:
- a) um salário fixo de dois salários mínimos a seus vendedores
- b) uma comissão fixa de R$ 50,00 por carro que for vendido
- c) caso o vendedor tenha vendido mais de 10 carros, uma comissão variável de 5% do
valor total de suas vendas.



### Exercício 09: Fatorial
Desenvolva um programa que calcule o fatorial de um numero inteiro N fornecido pelo usuário 

### Exercício 10: Tabuada 
Implemente um programa que que imprima a tabuada de um número fornrcido pelo usuário, de um 1 a 10.
