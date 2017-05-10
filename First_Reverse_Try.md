```c#
int[] firstReverseTry(int[] arr)
{
    if(arr.Length == 0) return arr;

    int x = arr[0];
    arr[0] = arr[arr.Length - 1];
    arr[arr.Length - 1] = x;
    return arr;

}
```
