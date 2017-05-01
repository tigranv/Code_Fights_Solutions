```c#
int countSumOfTwoRepresentations2(int n, int l, int r) {
    
    int count = 0;
    
    for(int i = l; i<=r; i++)
    {
      for(int j = i; j<=r&&n-j>=l; j++)
    {
     if(i+j == n)  count++;
    }  
        
    }

    return count;
}
```
