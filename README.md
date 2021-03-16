Bonjour,
Je m'appelle Louis, j'ai un problème de boucle imbriquée, je dois pouvoir réaliser un flocon (6 pointes) avec des étoiles et je ne comprend pas comment imbriquer les différentes fonctions pour avoir cette forme. (voir la capture d'écran pour mieux voir la forme recherché)
Merci pour vos retours _/\_

include <stdio.h>
#include <stdlib.h>

int main()
{
    int L, C;
    int i, j;
    printf("Veuillez saisir le nombre de lignes : ");
    scanf("%d", &L);
    printf("Veuillez saisir le nombre de colonnes : ");
    scanf("%d", &C);
    for (i = 1; i <= L; i++){
        for (j = 1; j <= C; j++){
            if (i == 1 || j <= i || i == L || j == C)
                printf("*");
            else
                printf(" ");
        }
    printf("\n");
    }
    return 0;
}
