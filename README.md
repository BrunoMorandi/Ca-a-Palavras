#include <stdio.h>
#include <stdlib.h>
#include <time.h>
#include <string.h>
int main(void)
{

int linha, coluna = 0, aux1, aux2, varRand, bRand;
int rand2, rand3, rand4, tema;

// ---------------------------------------------------------------------------------------------------------
// -------------------------TEMA 1 JOGOS--------------------------------------------------------------------

       char armas[5]={'a','r','m','a','s'};
       char black[5]={'b','l','a','c','k'};
       char sonic[5]={'s','o','n','i','c'};

// ---------------------------------------------------------------------------------------------------------
// -------------------------TEMA 2 ANIMES--------------------------------------------------------------------

       char kilua[5]={'k','i','l','u','a'};
       char light[5]={'l','i','g','h','t'};
       char mello[5]={'m','e','l','l','o'};

// ---------------------------------------------------------------------------------------------------------
//------------------------- TEMA 3 POKEMON-----------------------------------------------------------------
char pichu[5] = { 'p','i','c','h','u' };
char minum[5] = { 'm','i','n','u','m' };
char zubat[5] = { 'z','u','b','a','t' };
//- --------------------------------------------------------------------------------------------------------
//------------------------- TEMA 4 SISTEMAS-----------------------------------------------------------------

char macos[5] = { 'm','a','c','o','s' };
char linux[5] = { 'l','i','n','u','x' };
char chrome[6] = { 'c','h','r','o','m','e' };
//- --------------------------------------------------------------------------------------------------------
//------------------------- TEMA 5 CARROS-----------------------------------------------------------------
char dodge[5] = { 'd','o','d','g','e' };
char opala[5] = { 'o','p','a','l','a' };
char punto[5] = { 'p','u','n','t','o' };
//-----------------------------------------------------------------------------------------------------------

char matdark[10][10];
char matvisual[10][10] = {NULL}; // PASSA NULL PARA DEIXAR A MATRIZ DE CARACTERES VAZIA


//começar a colocar as palavras

srand(time(NULL));
varRand = rand()%4;
varRand += 1;

rand2 = rand()%4;
rand2 += 1;

rand3 = rand()%4;
rand3 += 1;

rand4 = rand()%2;
rand4 += 1;

bRand = rand()%9;
bRand++;
printf("%d \n ",bRand);
// funçao like a boss para sortear a s etras da matriz

for(linha = 0; linha < 10; linha ++)
{
for(coluna = 0; coluna < 10; coluna ++ )
{
if((matvisual[linha][coluna]) == NULL) // == para rodar normal
{
matvisual[linha][coluna ] = 102 + rand()%20;
}
}
}

    // -----------------------------------------------primeiro tema-------------------------------------------------
    if(bRand == 1)
    {
    printf("tema: jogo \n"); 
    // preenchendo com as palavras
//primeira palavra
       aux1 = 0;
coluna = bRand;
for(linha = varRand; aux1 < 5; linha ++)
{

           {
              matvisual[linha][coluna ] = armas[aux1]; // linha + coluna para ficar na diagonal
              aux1++;
   }
}
//condicoes
if(coluna >= 10)
{
coluna ++;
}
else
{
coluna -= 2;
}
// segunda palavra
       aux1 = 0;
for(linha= rand2; aux1<5; linha ++)
{
matvisual[linha][coluna] = black[aux1];
aux1 ++;
}

//condicoes
if(coluna >= 10)
{
coluna ++;
}
else
{
coluna -= 2;
}
// terceira palavra
aux1=0;
for(linha = rand3; aux1 < 5; linha ++)
{
matvisual[linha][coluna] = sonic[aux1];
aux1 ++;
} 
     
}
// -----------------------------------------------segundo tema-------------------------------------------------
if(bRand == 2)
{
printf("tema: animes \n");
// preenchendo com as palavras
       //primeira palavra
       aux1 = 0;
coluna = bRand;
for(linha = varRand; aux1 < 5; linha ++)
{

           {
              matvisual[linha][coluna ] = kilua[aux1]; // linha + coluna para ficar na diagonal
              aux1++;
   }
}
//condicoes
if(coluna >= 10)
{
coluna ++;
}
else
{
coluna -= 2;
}
// segunda palavra
       aux1 = 0;
for(linha= rand2; aux1<5; linha ++)
{
matvisual[linha][coluna] = light[aux1];
aux1 ++;
}

//condicoes
if(coluna >= 10)
{
coluna ++;
}
else
{
coluna -= 2;
}
// terceira palavra
aux1=0;
for(linha = rand3; aux1 < 5; linha ++)
{
matvisual[linha][coluna] = mello[aux1];
aux1 ++;
}
}
// -----------------------------------------------terceiro tema-------------------------------------------------
  if(bRand == 3)
    {
    printf("tema: pokemon \n"); 
    // preenchendo com as palavras
//primeira palavra
       aux1 = 0;
coluna = bRand;
for(linha = varRand; aux1 < 5; linha ++)
{

           {
              matvisual[linha][coluna ] = pichu[aux1]; // linha + coluna para ficar na diagonal
              aux1++;
   }
}
//condicoes
if(coluna >= 10)
{
coluna ++;
}
else
{
coluna -= 2;
}
// segunda palavra
       aux1 = 0;
for(linha= rand2; aux1<5; linha ++)
{
matvisual[linha][coluna] = minum[aux1];
aux1 ++;
}

//condicoes
if(coluna >= 10)
{
coluna ++;
}
else
{
coluna -= 2;
}
// terceira palavra
aux1=0;
for(linha = rand3; aux1 < 5; linha ++)
{
matvisual[linha][coluna] = zubat[aux1];
aux1 ++;
} 
     
}
// -----------------------------------------------quarto tema-------------------------------------------------
if(bRand == 4)
{
printf("tema: sistemas \n");
// preenchendo com as palavras
       //primeira palavra
       aux1 = 0;
coluna = bRand;
for(linha = varRand; aux1 < 5; linha ++)
{

           {
              matvisual[linha][coluna ] = macos[aux1]; // linha + coluna para ficar na diagonal
              aux1++;
   }
}
//condicoes
if(coluna >= 10)
{
coluna ++;
}
else
{
coluna -= 2;
}
// segunda palavra
       aux1 = 0;
for(linha= rand2; aux1<5; linha ++)
{
matvisual[linha][coluna] = linux[aux1];
aux1 ++;
}

//condicoes
if(coluna >= 10)
{
coluna ++;
}
else
{
coluna -= 2;
}
// terceira palavra
aux1=0;
for(linha = rand3; aux1 < 6; linha ++)
{
matvisual[linha][coluna] = chrome[aux1];
aux1 ++;
}
}
// -----------------------------------------------quinto tema-------------------------------------------------
  if(bRand >= 5)
    {
    printf("tema: carros \n"); 
    // preenchendo com as palavras
//primeira palavra
       aux1 = 0;
coluna = bRand;
for(linha = varRand; aux1 < 5; linha ++)
{

           {
              matvisual[linha][coluna ] = dodge[aux1]; // linha + coluna para ficar na diagonal
              aux1++;
   }
}
//condicoes
if(coluna >= 10)
{
coluna ++;
}
else
{
coluna -= 2;
}
// segunda palavra
       aux1 = 0;
for(linha= rand2; aux1<5; linha ++)
{
matvisual[linha][coluna] = opala[aux1];
aux1 ++;
}

//condicoes
if(coluna >= 10)
{
coluna ++;
}
else
{
coluna -= 2;
}
// terceira palavra
aux1=0;
for(linha = rand3; aux1 < 5; linha ++)
{
matvisual[linha][coluna] = punto[aux1];
aux1 ++;
} 
     
}
//-------------------------------------------printar------------------------------------------

       for(linha = 0; linha < 10; linha ++)
       {
           for(coluna = 0; coluna < 10; coluna++)
           {
               printf("%c  ",matvisual[coluna][linha]);
               }
           printf("\n");
       }

// declaracao de variaveis
       char chute[5];
       int acertou = 0,errou = 0;
//------------------------------------------------ chutes -------------------------------------------
       
      //---------------------- caso tema 1------------------------
if(bRand == 1)
{
do
       {
           printf("\t digite  chute: \n");
           scanf("%s", &chute);
               if(strcmp(chute, "armas") == 0 || strcmp (chute, "sonic") == 0 || strcmp(chute, "black") == 0)
               {
                   printf("acertou \n");
                   acertou ++;
               }
               else
               {
                   printf("errou \n");
                   errou ++;
               }
       }
while(acertou < 3); 
}
//---------------------- caso tema 2------------------------
if(bRand == 2)
{
do
       {
           printf("\t digite  chute: \n");
           scanf("%s", &chute);
               if(strcmp(chute, "kilua") == 0 || strcmp (chute, "light") == 0 || strcmp(chute, "mello") == 0)
               {
                   printf("acertou \n");
                   acertou ++;
               }
               else
               {
                   printf("errou \n");
                   errou ++;
               }
       }
while(acertou < 3); 
}
//---------------------- caso tema 3------------------------
   if(bRand == 3)
{
do
       {
           printf("\t digite  chute: \n");
           scanf("%s", &chute);
               if(strcmp(chute, "pichu") == 0 || strcmp (chute, "minum") == 0 || strcmp(chute, "zubat") == 0)
               {
                   printf("acertou \n");
                   acertou ++;
               }
               else
               {
                   printf("errou \n");
                   errou ++;
               }
       }
while(acertou < 3); 
}
//---------------------- caso tema 4------------------------
if(bRand == 4)
{
do
       {
           printf("\t digite  chute: \n");
           scanf("%s", &chute);
               if(strcmp(chute, "macos") == 0 || strcmp (chute, "linux") == 0 || strcmp(chute, "chrome") == 0)
               {
                   printf("acertou \n");
                   acertou ++;
               }
               else
               {
                   printf("errou \n");
                   errou ++;
               }
       }
while(acertou < 3); 
}
//---------------------- caso tema 5------------------------
if(bRand >= 5)
{
do
       {
           printf("\t digite  chute: \n");
           scanf("%s", &chute);
               if(strcmp(chute, "opala") == 0 || strcmp (chute, "dodge") == 0 || strcmp(chute, "punto") == 0)
               {
                   printf("acertou \n");
                   acertou ++;
               }
               else
               {
                   printf("errou \n");
                   errou ++;
               }
       }
while(acertou < 3); 
}
       return 0;
}

