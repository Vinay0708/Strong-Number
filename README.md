# Strong-Number
#include <stdio.h>
int main()
{   int n,abtakkaprod,abtakkasum=0,i,a,digit;
    printf("Enter a number that you want to check strong or not:\n");
    scanf("%d",&n);
    a=n;
    while(n>0)
    {
        digit=n%10;
        n=n/10;
        abtakkaprod=1;
        for(i=1; i<=digit; i++)
          abtakkaprod=abtakkaprod*i;
          abtakkasum=abtakkasum+abtakkaprod;
    }
    if(abtakkasum==a)
    printf("%d is strong number:",a);
    else
    printf("%d number is not strong:",a);
    return 0;
}
