#include<cs50.h>
#include<stdio.h>
void chart(int score);
int main(void)
{
    int scores[3];
    for(int i=0;i<3;i++)
    {
        scores[i]=get_int("score%i:",i+1);
    }
    
    for(int i=0;i<3;i++)
    {
        printf("score%i:",i+1);
        chart(scores[i]);
    }     
       

    
}

void chart(int score)
{
    for(int i=0; i<score; i++)
    {
        printf("*");
    }
    printf("\n");
}
    

