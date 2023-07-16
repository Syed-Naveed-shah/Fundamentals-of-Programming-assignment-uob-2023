#include <stdio.h>
int isprime(int number)
{
    int loop,count;
  if(number <=1)
  {
  return 0;
}
for(loop=2; loop*loop<=number; loop++)
{
if(number%loop==0)
{
return 0;
}
}
return 1;
}
int main()
{
    int num,store;
    printf("Enter a number between 2 to 100 : ");
    scanf("%d",&num);
    if(num>=2 && num<=100)
    {
        store=isprime(num);
        printf("%d",store);
    }
    else if(num==1)
    {
        printf("Kindly Enter a number between 2 to 100 : ");
        scanf("%d",&num);
        store=isprime(num);
        printf("%d",store);
    }
    else
    {
   
        printf("Number out of range");
   
}

}
