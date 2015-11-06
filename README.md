# MagicSquare_problem
# include &lt;stdio.h> 
# include &lt;conio.h> 
int main() 
{ int n, i, j, c, a[9][9] ;
printf("Enter the size of the magic square : ") ; 
scanf("%d", &amp;n) ;     
if (n % 2 == 0)     
{         printf("\nMagic square is not possible") ;          return 0;     } 
printf("\nThe magic square for %d x %d is :\n\n", n, n) ;
j = (n + 1) / 2 ;
i = 1 ;
for(c = 1 ; c &lt;= n * n ; c++)
{ 
a[i][j] = c ;
if(c % n == 0)
{                 i = (i + 1);              continue;             }
if(i == 1)  i = n ;
else  i = i - 1 ; 
if(j == n)   j = 1; 
else   j = j + 1 ; 
}
for (i = 1 ; i &lt;= n ; i++)
{
for (j = 1 ; j &lt;= n ; j++)
{             printf("%d\t", a[i][j]) ;             } 
printf("\n\n") ;
} 
return 0; 
}
