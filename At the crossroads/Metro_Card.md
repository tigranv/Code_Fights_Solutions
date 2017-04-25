```c#
int[] metroCard(int lastNumberOfDays) 
{
    if(lastNumberOfDays == 30 || lastNumberOfDays == 28)
    {
        int [] arr = new int[1];
        arr[0] = 31;
        return  arr;
    }
    
    else 
    {
       int [] arr1 = new int[3];
       arr1[0] = 28;
       arr1[1] = 30;
       arr1[2] = 31;
       return  arr1;
    }
}
```
