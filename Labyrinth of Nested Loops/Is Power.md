 ```c#
 bool isPower(int n)
{
    if (n == 1 || n == 2) return true;
    for (int i = 2; i <n; i++)
    {
        for (int j = 1; j < n; j++)
        {
            if (Math.Pow(i, j) > n) break;
            if (Math.Pow(i, j) == n) return true;                       
        }
    }
    return false;
}
```
