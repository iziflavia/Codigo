//Codigo - calculando linha em Matriz.

# include <stdio.h>
int main (){
    //Declarando variáveis.
       
    float m[12][12], x, soma=0, media=0;//NÚMEROS FLUTUANTES(REAIS).
    int L, i, j, a;//INTEIROS.
    char T;//CARACTERES.
       
    scanf("%d %c", &L, &T); /*Entrada do usuário "L" caractere com número inteiro que fará o calculo da linha, 
                              e "T" para informar se irá "SOMAR" ou fazer "MÉDIA".*/
                                       
    //Laço FOR incluindo os valores da Matriz.
    for(i=0; i<12; i++){
       for(j=0; j<12; j++){               
          scanf("%f", &m[i][j]);//Armazenamento.
          }
          }
       for(a=0; a<12; a++){ //Irá exibir a matriz.
          soma = soma+m[L][a]; //Somando os valores da linha, conforme solicitado pelo usuário.
          }
           
       if(T=='S')//Condição, caso for 'S', irá somar a linha.
          printf("%.1f\n", soma);//Impressão na tela.
          
             
       if(T=='M')//Condição, caso for, 'M', irá fazer a média da linha.
          printf("%.1f\n", soma/12);//Impressão na tela.
 
    return 0;
}
