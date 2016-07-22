#include<stdio.h>
void dup(char *a)
int main()
{
char a[10];
scanf("%s",a);
dup(a);
printf("%s",a);
return 0;
}
void dup(char *a)
{
int n,i,k;
n=strlen(a);
for(i=0;i<n;i++)
{
for(j=k=i+1;k<=n;)
{
if(a[i]!=a[j])
{
a[j]=a[k];
j++;
k++;
}else
k++;
}
}
}
