# conversion-of-temperature-
#include <stdio.h>
int main()
{
    float celsius, fahrenheit;
    int ch; 
    printf("1.fahrenheit to celsius\n2.celsius to fahrenheit\n3.exit\n");
    while(1)
    {
      printf("enter choice");
      scanf("%d",&ch);
        switch(ch)
        {
            case 1:
            printf("Enter temperature in Fahrenheit:");
            scanf("%f",&fahrenheit);
            celsius = (fahrenheit - 32) * 5 / 9;
            printf("%f\n",celsius);
            break;
            case 2:
            printf("Enter temperature in celsius:");
            scanf("%f",&celsius);
            fahrenheit = (celsius * 9 / 5) + 32;
            printf("%f\n",fahrenheit);
            break;
            case 3:exit(1);
            break;
        }
    }
    return 0;
}
