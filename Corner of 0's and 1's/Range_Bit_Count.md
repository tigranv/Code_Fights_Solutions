```c#
int rangeBitCount(int a, int b) {
    int ones = 0;
    for(int i = a; i <=b; i++){
        int s = i;
        while(s > 0){
            ones += s & 1;
            s = s >> 1;
        }
    }
    return ones;
}
```
