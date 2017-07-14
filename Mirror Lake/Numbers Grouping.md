```c#
int numbersGrouping(int[] a)
{
    Array.Sort(a);
    int count = 0;
    int i = 0;
    int j = 1;
    do
    {
        if ((i < a.Length) && (a[i] <= j * 10000) && (a[i] >= (j - 1) * 10000 + 1)) count++;
        while ((i < a.Length) && (a[i] <= j * 10000) && (a[i] >= (j - 1) * 10000 + 1))
        {
            i++;
        }          
        j++;
    } while (i<a.Length);

    return count + a.Length;
}
```
