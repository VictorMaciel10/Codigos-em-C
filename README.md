**Exercício 1 

-----------------CLASSIFICAÇÃO DE IDADE----------------

#include <stdio.h>
#include <stdlib.h>

int main() {
    int idade;

    printf("Por favor, diga sua idade: ");
    scanf("%d", &idade);

    if (idade < 18) {
        printf("Menor de idade\n");
    } else if (idade >= 18 && idade <= 64) {
        printf("Adulto, Gente grande!\n");
    } else {
        printf("Idoso\n");
    }

    return 0;
}

**Exercício 2

-------------------CÁLCULO DE MEDIA E AVALIAÇÃO DE DESEMPENHO--------------------

#include <stdio.h>
#include <stdlib.h>
int main() {
    float nota1, nota2, nota3, media;

    printf("Diga a primeira nota: ");
    scanf("%f", &nota1);

    printf("Diga a segunda nota: ");
    scanf("%f", &nota2);

    printf("Diga a terceira nota: ");
    scanf("%f", &nota3);

    media = (nota1 + nota2 + nota3) / 3;

    printf("Media: %.2f\n", media);

    if (media >= 7) {
        printf("Parabens!Aprovado\n");
    } else if (media >= 5 && media < 7) {
        printf("Que pena!Recuperacao\n");
    } else {
        printf("Sinto Muito,Reprovado\n");
    }

    return 0;
}

**Exercício 3

--------------CALCULADORA SIMPLES---------------
#include <stdio.h>
#include <stdlib.h>

int main() {
    float num1, num2, resultado;
    char operacao;

    printf("Digite o primeiro numero, por favor: ");
    scanf("%f", &num1);

    printf("Digite a operacao (+, -, *, /): ");
    scanf(" %c", &operacao);

    printf("Agora, digite o segundo numero: ");
    scanf("%f", &num2);

    if (operacao == '+') {
        resultado = num1 + num2;
        printf("%.2f + %.2f = %.2f\n", num1, num2, resultado);
    } else if (operacao == '-') {
        resultado = num1 - num2;
        printf("%.2f - %.2f = %.2f\n", num1, num2, resultado);
    } else if (operacao == '*') {
        resultado = num1 * num2;
        printf("%.2f * %.2f = %.2f\n", num1, num2, resultado);
    } else if (operacao == '/') {
        if (num2 != 0) {
            resultado = num1 / num2;
            printf("%.2f / %.2f = %.2f\n", num1, num2, resultado);
        } else {
            printf("Erro: Divisão por zero!\n");
        }
    } else {
        printf("Erro: Operação inválida!\n");
    }

    return 0;
}

Exercício 4

-------------- TABUADA DE UM NÚMERO--------------------

#include <stdio.h>
#include <stdlib.h>

int main() {
    int numero, i;

    printf("Digite um numero inteiro: ");
    scanf("%d", &numero);

    printf("Tabuada de %d:\n", numero);

    for (i = 1; i <= 10; i++) {
        printf("%d x %d = %d\n", numero, i, numero * i);
    }

    return 0;
}

Exercício 5 

------------------ NUMEROS PARES ENTRE 1 E N---------------------

#include <stdio.h>
#include <stdlib.h>

int main() {
    int N, i;

    printf("Digite um numero inteiro positivo: ");
    scanf("%d", &N);

    printf("Numeros pares entre 1 e %d:\n", N);

    for (i = 1; i <= N; i++) {
        if (i % 2 == 0) {
            printf("%d\n", i);
        }
    }

    return 0;
}
