```c#
int leastFactorial(int n) {

    int i = 1;
    int f = 1;
    
    while (f<n)
    {                
     f=f * i;
     i++;

    }
    
    return f;
}
```
