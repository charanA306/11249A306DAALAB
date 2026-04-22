#include<stdio.h>

void toh(int n,char s,char d,char a)
{
  if(n==1)
    {
      printf("\nmove disk %d from %c to %c" , 1, s, d);
      return ;
    }
    
    toh(n-1, s, a, d);
    
    printf("\nmove disk %d from %c to %c ", n, s, d);
    
    toh(n-1, a, d, s);
}

int main()
{
  int n;
  printf("enter no of disks:");
  scanf("%d",&n);
  
  toh(n,'S','D','A');
  
  return 0 ;
}
