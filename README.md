# Exercicis-basicos-resolvidos
Alguns Exercícios das aulas do primeiro semestre da Faculdade resolvidos

/*Exercicio = 01 sucessor e anteccessor*/

#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

int main()
{
    int num1, ante, sucess;

    setlocale(LC_ALL,"portuguese");
    printf("Digite um numero inteiro:\n");
    scanf("%d", &num1);
    sucess = num1 + 1;
    ante = num1 - 1;
    printf("\nVocê digitou  %d ", num1);
    printf("\nEsse é o seu sucessor  %d ", sucess);
    printf("\nEsse é o seu antecessor %d ", ante);

    return 0;
}

/*Exercicio = 02 Quinta parte de um numero*/

#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

 int main()
{
    float num1, quinta ;

    setlocale(LC_ALL,"portuguese");
    printf("Digite um numero :\n");
    scanf("%f", &num1);
    quinta = num1 / 5;

    printf("\nVocê digitou  %.2f \n", num1);
    printf("\nEssa é a sua quintaparte  %.2f \n", quinta);


    return 0;
}

Exercicio = 03 soma de tres numeros

#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

 int main()
{
    int num1, num2, num3, soma ;

    setlocale(LC_ALL,"portuguese");
    printf("Digite 3 numeros inteiros :\n");
    scanf("%d%d%d", &num1, &num2, &num3);

    soma = num1 + num2 + num3;

    printf("\nVocê digitou  %d %d %d \n", num1,num2,num3);
    printf("\nA soma dos 3 numeros digitados é %d\n", soma);


    return 0;
}

/*Exercicio = 04 media*/

#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

 int main()
{
    float num1, num2, num3, num4, media ;

    setlocale(LC_ALL,"portuguese");
    printf("Digite 4 valores :\n");
    scanf("%f%f%f%f", &num1, &num2, &num3, &num4);

    media = (num1 + num2 + num3 + num4) / 4;

    printf("\nVocê digitou  %.2f %.2f %.2f %.2f \n", num1,num2,num3,num4);
    printf("\nA media dos 4 valores digitados é %.2f\n", media);


    return 0;
}

/*Exercicio = 05 Nascimento*/

#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

 int main()
{
    int idade, nasci ;

    setlocale(LC_ALL,"portuguese");
    printf("Digite sua idade:\n");
    scanf("%d", &idade);

    nasci = 2020 - idade;

    printf("\nVocê nesceu em %d\n", nasci);



    return 0;
}

/* Exercicio = 06 Km/h convertido por m/s */

#include <stdio.h>

int main () {

	float km, ms;

	printf("Digite uma velocidade em Km/h: ");
	scanf("%f", &km);

	ms = km/3.6; // 1 hora contem 3600 segundos.

	printf("\n%2.f Km/h convertido para %2.fm/s\n", km, ms);


	return 0;

}

 /*Exercicio = 07 Cotação do dolar*/

#include <stdio.h>
#include <stdlib.h>

int main()
{
    float dolar = 5.30, real, resultado;
    printf("\nDigite um valor em reais $");
    scanf("%f",&real);
    resultado = (real / dolar);
    printf("\n%.2f",resultado);
    return 0;
}

/*EXERCICIO = 08 TEMPERATURA*/

#include <stdio.h>
#include <stdlib.h>
#include <math.h>
/*Ler uma temperatura em graus Celsius e apresentá-la convertida em graus Fahrenheit. A
fórmula de conversão é: 𝐹 = 𝐶 ∗ (9,05,0) + 32,0, sendo 𝐹 a temperatura em Fahrenheit e 𝐶 a
temperatura em Celsius*/

int main() {
    float c, f;
    printf("Digite a temperatura em Graus Celsius: ");
    scanf("%f", &c);
    f = c*(9.0/5.0) + 32.0;
    printf("\nA temperatura em Fahrenheit eh: %.2f", f);
    return 0;
}


/*EXERCICIO = 10 dIVISÃO ENTRE GANHADORES*/

#include <stdio.h>
#include <stdlib.h>
/* A importância de R$ 780.000,00 será dividida entre três ganhadores de um concurso.
Sendo que da quantia total:
 O primeiro ganhador receberá 46%;
 O segundo receberá 32%;
 O terceiro receberá o restante;
Calcule e imprima a quantia ganha por cada um dos ganhadores. */

int main() {
    float valor = 780.000;
    printf("O valor total eh:R$%.3f", valor );
    float gan1, gan2, desc2, gan3, desc3;
    gan1=  valor * 0.46;
    printf("\nPrimeiro ganhador recebe:R$%.3f", gan1);
    gan2=  valor * 0.32;
    printf("\nPrimeiro ganhador recebe:R$%.3f", gan2);
    gan3=  valor * 0.22;
    printf("\nPrimeiro ganhador recebe:R$%.3f", gan3);
    printf("\n\n");
    system("pause");
    return 0;
}


/*Exercicio = 12 Altura e raio de um cilindro*/

#include <stdio.h>
#include <stdlib.h>
/* . Leia a altura e o raio de um cilindro circular e imprima o volume do cilindro. O volume de
um cilindro circular é calculado por meio da seguinte fórmula: V = ?? * ????????2* ????????????, onde?? = 3,141592 .*/

int main() {
    int altura = 4;
    printf("A altura do cilindro eh: 4");
    int raio = 2;
    printf("\nO raio do cilindro eh: 2");
    float volume = 3.14 * (raio*raio) * altura;
    printf("\nO volume do cilindro eh: %.2f" , volume);
    printf("\n\n");
    system("pause");
    return 0;
}

/*Exercicio = 14 Letra minuscala em letra maiuscula*/

#include <stdio.h>
#include <stdlib.h>
#include <ctype.h>
/*  Faça um programa para converter uma letra maiúscula em letra minúscula. Use a tabela
ASCII. */

int main(void) {
    char letra;
    printf("Digite uma letra minuscula: ");
    scanf("%c", &letra);
    letra = toupper(letra);
    printf("\nLetra em maiusculo: %c " , letra);
    printf("\n");
    system("pause");
    return 0;
}
