```c#
int mirrorBits(int a) {    
  return Convert.ToInt32(new String(Convert.ToString(a, 2).Reverse().ToArray()), 2);
}
```
