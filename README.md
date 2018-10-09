#include <stdio.h>

int main(){

    int riadok,stlpec,r,p,v,s;
    scanf("%d",&p);
    for (int k = 1; k <=p ; k++) {
        scanf("%d %d %d", &v, &s, &r);
        for (int i = 1; i <= v; i++) {
            for (riadok = 1; riadok <= r; riadok++) {
                for (int j = 1; j <= s; j++) {
                    for (stlpec = 1; stlpec <= r; stlpec++) {
                        if(riadok>=stlpec)
                            printf("*");
                        else
                            printf(" ");
                    }
                }
                printf("\n");
            }
        }
    }
    return 0;
}
