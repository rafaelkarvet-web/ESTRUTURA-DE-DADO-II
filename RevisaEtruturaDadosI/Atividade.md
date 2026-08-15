SISTEMA DE PROGRAMACAO EM ESTRUTURA DE DADOS 2 EM C++
CALCULADORA:
```
#include <stdio.h>

float Somar(float Num1, float Num2);
float Subtrair(float Num1, float Num2);
float Multiplicar(float Num1, float Num2);
float Dividir(float Num1, float Num2);

int main () {
	float vlr1, vlr2;
	printf ("informe o primeiro valor: ");
	scanf("%f", &vlr1);
	printf ("informe o segundo valor: ");
	scanf("%f", &vlr2);
	
	printf("\n a somar de %0.1f + %0.1f = %0.1f", vlr1, vlr2, Somar(vlr1, vlr2));
	
	printf("\n a Subtracao de %0.1f - %0.1f = %0.1f", vlr1, vlr2, Subtrair(vlr1, vlr2));
	
	printf("\n a Multiplicao de %0.1f * %0.1f = %0.1f", vlr1, vlr2, Multiplicar(vlr1, vlr2));
	
	printf("\n a Divisao de %0.1f / %0.1f = %0.1f", vlr1, vlr2, Dividir(vlr1, vlr2));
	
	
	
}
float Somar(float Num1, float Num2) {
  float Resultado;
  Resultado = Num1+Num2;
  return(Resultado);
}

float Subtrair(float Num1, float Num2) {
  float Resultado;
  Resultado = Num1-Num2;
  return(Resultado);
}

float Multiplicar(float Num1, float Num2) {
  float Resultado;
  Resultado = Num1*Num2;
  return(Resultado);
}
float Dividir(float Num1, float Num2) {
  float Resultado;
  Resultado = Num1/Num2;
  return(Resultado);
}
```
SISTEMA DE PROGRAMACAO EM ESTRUTURA DE DADOS 2 EM C++
INSERCAO:
```

#include <stdio.h>

int vetor[5]={5,3,1,4,2};

int main () {

  int qtd=5,i,j,aux,trocas;
  printf("\n vetor original:");
  for (i=0; i<qtd; i++)
  printf("%i, ",vetor[i]);
 trocas =0;
 
 for(i=1; i<qtd; i++){
 	aux = vetor[i];
 	j=i-1;
 	while(j>=0 && aux<vetor[j]){
 		vetor[j+1] = vetor[j];
 		j--;
 		trocas++;
	 }
	 vetor[j+1] = aux;
 }    
   
   
   printf ("\n vetor ordenada : ");
   for (int i=0; i<qtd; i++)
   printf ("%i, " ,vetor[i]);
   printf("\n total trocas: %i", trocas);
   
      printf ("\n vetor decrescente : ");
   for (int i=14; i>=0; i--)
   printf ("%i, " ,vetor[i]);


}
```
