#include <stdio.h>
int a[50];
void sort(int[],int);
int main()
{
    int i,n;
    printf ("enter the no of elemnts");
    scanf ("%d",&n);
    printf("enter the  elements");
    for (i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    sort(a,n);
    for(i=0;i<n;i++)
    {
        printf("%d",a[i]);
    }
}
void sort(int a[], int n)
{
    int i,j, temp,flag=0;
    for (i=0;i<n-1;i++)
    {
        flag =0;
        for(j=0;j<n-i-1;j++)
        {
           if (a[j] > a[j+1])
           {
            temp = a[j];
            a[j]=a[j+1];
            a[j+1]=temp;
            flag = 69;
           }
           }
           if (flag==0);
           break;
           
    }
}

