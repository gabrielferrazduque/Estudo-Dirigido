# Estudo-Dirigido
Estudo Dirigido
#include <stdio.h>

// Função que imprime os números de 1 a 100 separados por vírgula
void imprimir_1_a_100() {
    for (int i = 1; i <= 100; i++) {
        if (i < 100) {
            printf("%d, ", i);
        } else {
            printf("%d\n", i);
        }
    }
}

// Função que calcula o somatório de todos os números ímpares entre 10 e 1000
void somatorio_impares() {
    int soma = 0;
    for (int i = 11; i < 1000; i += 2) {
        soma += i;
    }
    printf("Somatório dos números ímpares entre 10 e 1000: %d\n", soma);
}

// Função que imprime todos os números múltiplos de 3 que não terminem em 3 entre 1 e 200
void multiplos_de_3_nao_terminados_em_3() {
    int primeiro = 1;
    for (int i = 3; i <= 200; i += 3) {
        if (i % 10 != 3) {
            if (primeiro) {
                printf("%d", i);
                primeiro = 0;
            } else {
                printf(", %d", i);
            }
        }
    }
    printf("\n");
}

int main() {
    imprimir_1_a_100();
    somatorio_impares();
    multiplos_de_3_nao_terminados_em_3();

    return 0;
}
