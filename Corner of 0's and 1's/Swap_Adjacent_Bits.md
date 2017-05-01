```c#
int swapAdjacentBits(int n)
{
  return ((n & 0x2AAAAAAA) >> 1) | (( n & 0x55555555) << 1);
}
```
