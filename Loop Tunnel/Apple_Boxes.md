```c#
int appleBoxes(int k)
{
    int r = 0;
    int y = 1;
    for (int i = 2; i <= k; i++)
    {
        y = i % 2 != 0 ? (y + i * i) : y;
        r = i % 2 != 0 ? r : (r + i * i);
    }
    return r - y;
}
```
