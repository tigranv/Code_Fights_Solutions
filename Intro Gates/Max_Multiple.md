```c#
int maxMultiple(int divisor, int bound) {
    int i = divisor;
    for(; i <= bound; i+= divisor);
    return i - divisor;
}
```
