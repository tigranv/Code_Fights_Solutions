```c#
int arrayPacking(int[] a) 
{
    int x = 0;
    for (int j = 0; j < a.Length; j++)
    {
        for (int i = 0; i < 8; i++)
        {
            if ((a[j] & (1 << i)) != 0)
            {
                x |= (1 << (i+8*j));
            }
        }
    }
    
    return x;
}
```
