```c#
int[] replaceMiddle(int[] arr) {
    
    int[] nearr = new int[arr.Length-1];
    
 if(arr.Length%2 == 0)
{

    for(int i =0; i< nearr.Length; i++)
    {
        if(i < arr.Length/2-1)
        {nearr[i] = arr[i]; }
            
        
        nearr[arr.Length/2-1] = arr[arr.Length/2 -1] + arr[arr.Length/2];
        
        if(i > arr.Length/2-1)
        {nearr[i] = arr[i+1]; }
            
    }
    
 return nearr;
    
}
```
