```c#
int isSumOfConsecutive2(int n)
{
    int test = 0;
    int[] arr = new int[n];
    for (int i = 0; i < n; i++)
    {
        arr[i] = i;
    }

    for (int j = 1; j < n; j++)
    {
        int sum = 0;
        for (int i = j; i < n; i++)
        {
            if (sum == n)
            {
                test++;
            }
            sum += arr[i];
        }
    }
    return test;
}
```
