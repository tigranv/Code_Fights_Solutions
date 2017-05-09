```c#
int countBlackCells(int n, int m)
{
    int c = 0;
    int x = 0;

    if (n > m)
    {
        c = (n % m == 0)?(n / m):(n / m + 1);
    }

    if (n < m)
    {
        c = (m % n == 0)?(m / n):(m / n + 1);
    }

    x = (n > m)?(n - 1):((m - 1) * c);

    if (n == m) x = m + 2*(m-1); 


    return x;
}
```
