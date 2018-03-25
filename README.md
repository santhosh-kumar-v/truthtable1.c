#include<stdio.h>
int main()
{
   int d[10][10][10],a,b,c;
   printf ("a\t\tb\t\tc\t\ta+(b+c)\n");
   for (a=0;a<=1;a++)
    {
        for (b=0;b<=1;b++)
        {
            for (c=0;c<=1;c++)
            {
                d[a][b][c]=(a||(b||c));
                printf ("%d\t\t%d\t\t%d\t\t%d\n",a,b,c,d[a][b][c]);
            }
        }
    }
}
