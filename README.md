# program
--------------------
1.Static Array
```c
#include <stdio.h>

int main()
{
    int arr[10];
    
    for(int i=0;i<sizeof(arr)/sizeof(1);i++){
        scanf("%d",&arr[i]);
    }
    
    for(int i=0;i<sizeof(arr)/sizeof(1);i++){
        printf("%d ",arr[i]);
    }
}
```
------------------------------------------------------------------------------
2.Dynamic Array
```c
#include <stdio.h>

int main()
{
    int arr[20],n;
    
    printf("Enter the Aray Limit:");
    
    scanf("%d",&n);
    
    for(int i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    
    printf("The elements are:\n");
    
    for(int i=0;i<n;i++){
        printf("%d ",arr[i]);
    }
}
```
-------------------------------------------------------------------------------------------------------------------
3.Sum of Array
```c
#include <stdio.h>

int main()
{
    int arr[5],sum=0;

    printf("Enter the Array Elements");
    
    for(int i=0;i<sizeof(arr)/sizeof(arr[0]);i++){
        scanf("%d",&arr[i]);
    }
    
    
    for(int i=0;i<sizeof(arr)/sizeof(arr[0]);i++){
        sum+=arr[i];
    }
    
    printf("The Sum=%d",sum);
}
```
--------------------------------------------------------------------------------------------------------------------------------------------
4.Product of Array
```c
#include <stdio.h>

int main()
{
    int arr[5],Product=1;

    printf("Enter the Array Elements:\n");
    
    for(int i=0;i<sizeof(arr)/sizeof(arr[0]);i++){
        scanf("%d",&arr[i]);
    }
    
    
    for(int i=0;i<sizeof(arr)/sizeof(arr[0]);i++){
        Product*=arr[i];
    }
    
    printf("The Product=%d",Product);
}
```
----------------------------------------------------------------------------------------------------------------------------
5.Sum of Odd and Even Position
```c
#include <stdio.h>

int main()
{
    int arr[10]={1,2,3,4,5,6,7,8,9,10},so=0,se=0;
    
    
    for(int i=0;i<sizeof(arr)/sizeof(arr[0]);i++){
        
        if((i+1)%2==0){
            se+=arr[i];
        }
        else{
            so+=arr[i];
        }
    }
    
    printf("The Sum of Odd=%d\nThe Sum of Even=%d",so,se);
}
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
### 6.Min and Max in the Array
```c
#include <stdio.h>

int main()
{
    int arr[10]={1,2,3,4,5,6,7,8,9,10},min,max;
    
    min=max=arr[0];
    
    for(int i=1;i<sizeof(arr)/sizeof(arr[0]);i++){
        
        if(arr[i]<min){
            min=arr[i];
        }
        else{
            max=arr[i];
        }
    }
    
    printf("Min=%d\nMAx=%d",min,max);
}
```
--------------------------------------------------------------------------------------------------------------------------------------------
