```c#
int rounders(int value) {
    int e = 1;
    
    while(value / 10 != 0){
        if(value % 10 >= 5){
            value/= 10;
            value++;
        }
        else{
            value/=10;
        }
        e *=10;
    }
    return value*e;
}
```
