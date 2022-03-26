	#include<stdio.h>
	
	int find_sum(int a, int mod);   // function prototype declaration
	
	int main()
	{
	    int a,digit,mod;
	    printf("enter any digit number except single digit");
	    scanf("%d",&a);
	    digit=find_sum(a,mod);
	    
	}
	
	int find_sum(int a, int mod) // function definition
	{
	   static int add=0;
	   while (a!=0) 
	    {
	        mod=a%10;
	        a=a/10;
	        add=add+mod;
	    }
	    printf("\nthe sum of digits is%d",add);
	    return 0;
	}
