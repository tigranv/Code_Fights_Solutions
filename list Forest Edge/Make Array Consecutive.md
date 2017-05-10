```c#
int makeArrayConsecutive2(int[] sequence) {
    
    Array.Sort(sequence);
    int count =0;
    
    for(int i =1; i< sequence.Length; i++)
    {
        if((sequence[i] - sequence[i-1]) !=0)
            count = count + (sequence[i] - sequence[i-1] -1);
    }
    
    return count;

}
```
