# PROVA :pencil: 

### Exercício 01: Solucione o erro

```c 
// Corrija o seguinte código para que ele imprima números impares menores que 10

#include <stdio.h>

int main()
{
  for (int i = 0; i < 10; i++)
  {
    if(i % 2 == 1)
    {
       printf("%d\n", i);
    }

  }
  return 0;
}
```
### Exercício 02: Determinar o maior 
Escreva um programa que receba três números e determina qual é o maior.

#include <stdio.h>

int main() {
    int num1, num2, num3;

    printf("Digite o primeiro número: ");
    scanf("%d", &num1);

    printf("Digite o segundo número: ");
    scanf("%d", &num2);

    printf("Digite o terceiro número: ");
    scanf("%d", &num3);
    
    if (num1 >= num2 && num1 >= num3) {
        printf("%d é o maior número.\n", num1);
    } else if (num2 >= num1 && num2 >= num3) {
        printf("%d é o maior número.\n", num2);
    } else {
        printf("%d é o maior número.\n", num3);
    }

    return 0;
}

### Exercício 03: Palíndromos
Palíndromos são números que têm o mesmo valor se lidos da esquerda para a direita
ou da direita para a esquerda. Exemplos: 44, 232, etc. Faça um programa que determine
e escreva todos os números inteiros entre 1000 que 10000 que são palíndromos.

#include <stdio.h>
int Palindromo(int num) {
    int reverso = 0;
    int original = num;

    while (num != 0) {
        int digito = num % 10;
        reverso = reverso * 10 + digito;
        num /= 10;
    }

    return reverso == original;
}

int main() {
    for (int i = 1000; i <= 10000; i++) {
        if (Palindromo(i)) {
            printf("%d\n", i);
        }
    }

    return 0;
}


### Exercício 04: Árvore
Faça um programa que imprima uma árvore de Natal, considerando uma altura
especificada pelo usuário. Para h=3:
```
  I
 *I*
**I**
```
#include <stdio.h>

int main() {
    int altura, espacos, asteriscos;

    printf("Altura da árvore: ");
    scanf("%d", &altura);
    for (int linha = 1; linha <= altura; linha++) {
        espacos = altura - linha;
        for (int i = 0; i < espacos; i++) {
            printf(" ");
        }
        asteriscos = 2 * linha - 1;
        for (int i = 0; i < asteriscos; i++) {
            printf("*");
        }
        printf("\n");
    }
    for (int i = 0; i < altura - 1; i++) {
        printf(" ");
    }
    printf("|\n");
    return 0;
}

### Exercício 05: Corriga o código 

```c 
// Corrija o seguinte código para que ele imprima números impares menores que 10

#include <stdio.h>

int main()
{
  int i,j;

  // Erro 1: Loop infinito
  for (i = 0; i < 10; i++)
  if(i % 2 == 1)
  {
    printf("i = %d\n", i);
  }
}
  // Erro 2: Condição de loop incorreta
  for (j = 0; j < 10; j += 2)
  {
    printf("j = %d\n", j);
  }
}
  // Lógica de verificação de número primo incorreta
  int num = 7, primo = 1;
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

#include <stdio.h>

int main() {
    int i, num;
    float soma = 0.0;
    int max, min;

    printf("Digite 10 números:\n");

     for (i = 0; i < 10; i++) {
        printf("Número %d: ", i + 1);
        scanf("%d", &num);
        if (i == 0) {
            max = num;
            min = num;
        } else {
            if (num > max) {
                max = num;
            }
            if (num < min) {
                min = num;
            }
        }
        soma += num;
    }
    float media = soma / 10.0;
    printf("Média: %.2f\n", media);
    printf("Máximo: %d\n", max);
    printf("Mínimo: %d\n", min);

    return 0;
}

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
    if(num % 2 == 0)
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

#include <stdio.h>

int main() {
    
    return 0;
}

### Exercício 09: Fatorial
Desenvolva um programa que calcule o fatorial de um numero inteiro N fornecido pelo usuário 

#include <stdio.h>
int main() {
int num, fat = 1; 
   scanf("%d",&num);
   for(int i=1; i<num; i++){
     fat= fat * i;
     printf("%d %d", num,fat);
   }
    return 0;
}

### Exercício 10: Tabuada 
Implemente um programa que que imprima a tabuada de um número fornrcido pelo usuário, de um 1 a 10.
#include <stdio.h>
int main() {
int num= 0
  printf("Digite o número: ");
  scanf(%d", &num);
  printf(num);
  for(int i = 1; i <=10; i++) {
    print(%d x %d = %d\n", num, i, num * i);
  }

    return 0;
}
