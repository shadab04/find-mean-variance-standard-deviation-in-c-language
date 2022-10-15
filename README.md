# find-mean-variance-standard-deviation-in-c-language
#include<stdio.h>
#include<math.h>
int main()
{
    int a[100],sum=0,mean,sum1,var,sd,variance;
    int i,n,k,j;
    printf("enter the size:");
    scanf("\n%d",&n);
    for(i=0; i<n; i++)
    {
        printf("enter element:");
        scanf("\n%d",&a[i]);
    }
    for(j=0; j<n; j++)
    {
      sum=sum+a[j];
    }
    printf("sum is %d",sum);
    mean=sum/n;
    for(k=0;k<n;k++)
    {
        sum1=sum1+(mean-a[k])*(mean-a[k]);
    }
    var=sum1/n;
    printf("\n variance is %d",var);
    sd=sqrt(var);
    printf("\n mean is %d",mean);
    printf("\n deviation is %d",sd);
    return 0;
}
