# Guess-Game
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() {
    int guess, number, nguesses=1;
    srand (time (0));
    number = rand()%100+1;

    do{
printf("Guess the Any Number between 1 to 100\n");

scanf("%d",&guess);

if(guess>number)

    printf("Lower Number Please !\n");

else if(guess<number)

    printf("Higher Number Please !\n");

else 
    printf("You Guesses the  Number  in %d Attempt \n",nguesses);
   nguesses ++; }
    
    while(guess!=number);
  
    
    return 0;
}
