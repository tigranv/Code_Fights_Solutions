```c#
int candles(int A, int B)
{
    int burned = 0;
    int leftowers = 0;
    while (A > 0)
    {
        burned += A;
        leftowers += A;
        A = leftowers / B;
        leftowers %= B;
    }
    return burned;
}
```
