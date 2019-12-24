# butterfly.c
program for butterfly pattern
#include <stdio.h>

int main(void) {
	int i,j,n;
	scanf("%d\n",&n);
			for(i=1;i<=n;i++)
	{
	    for(j=1;j<=2*n;j++)
	    {
	        if((j<=i) || (j>2*n-i))
	        {
	            printf("*\t");
	        }
	        else
	        printf("\t");
	    }
	    printf("\n");
	}
	for(i=1;i<=n;i++)
	{
	    for(j=1;j<=2*n;j++)
	    {
	        if((j<=n-i+1) || (j>n+i-1))
	        {
	            printf("*\t");
	        }
	        else
	        printf("\t");
	    }
	    printf("\n");
	}
	
	return 0;
}
