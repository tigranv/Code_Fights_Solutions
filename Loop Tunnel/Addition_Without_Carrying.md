```c#
int additionWithoutCarrying(int param1, int param2)
{
    int l1 = param1 >= param2? param1.ToString().Length : param2.ToString().Length;
    int x = 0;

    for (int i = 0; i < l1; i++)
    {
        x = x + ((param1 % 10 + param2 % 10) % 10) * (int)Math.Pow(10, i);
        param1 = param1 / 10;
        param2 = param2 / 10;
    }
    return x;
}
```
        
