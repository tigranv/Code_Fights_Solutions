```c#
int lineUp(string commands) {
    int s = 0;
    bool same = true;
    
    foreach(char c in commands)
    {
        switch(c)
        {
            case 'A':
                break;
            default:
                same ^= true;
                
                break;
        }
        if(same)
            s++;
    }
    
    return s;
}
```
