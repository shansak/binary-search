
#include<stdio.h>
#include<conio.h>

void binary(int a[],int n,int x)
{   int mid;
    int start=0;
    int end=n-1;

    while(start<=end)
    {
     mid=(start+end)/2;
     if(x==a[mid])
     {
         printf("got item at %d",mid);
         return;
     }
     else if(a[mid]>x)


        end=mid-1;

     else
        start=mid+1;

    }
    printf("stop");



}

void main()
{
    int a[]={3,15,27,30,41,90,95,300,400};

    binary(a,9,95);
}
