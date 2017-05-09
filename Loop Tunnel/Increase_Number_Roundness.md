```c#
bool increaseNumberRoundness(int n)
{
    bool bo = false;
    while (n%10 == 0) n = n / 10;
    while (n > 9)
    {
        if (n%10 != 0) n = n / 10;

        else
        {
            bo = true;
            break;
        }
    }

    return bo;
}
```
