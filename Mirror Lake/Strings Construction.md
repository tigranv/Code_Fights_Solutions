```c#
int stringsConstruction(string A, string B) {
    int num = 0;
    List<char> available = B.ToList();
    
    while(available.Count > 0)
    {
        foreach(char c in A)
        {
            if(!available.Remove(c))
                return num;
        }
        num++;
    }
    return num;
}
```
