# reversing-array-elements.c
//  C program of reversing array elements.
//  C program of reversing array elements
#include <stdio.h>

int main() {
    int i,n,t;
    int a[]={2,4,6,8,10,12,14,16};
    printf("BEFORE REVERSING =\n");
    for(i=0;i<8;i++)
     printf("%d\n",a[i]);
    n=8;
    for(i=0;i<n/2;i++){
        t=a[i];
        a[i]=a[n-1-i];
        a[n-1-i]=t;
    }
    printf("AFTER REVERSING =\n");
    for(i=0;i<8;i++)
     printf("%d\n",a[i]);
    return 0;
}
