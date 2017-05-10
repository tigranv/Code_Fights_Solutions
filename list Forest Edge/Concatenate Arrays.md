```c3
int[] concatenateArrays(int[] a, int[] b) {
    
     if((a.Length == 0) && (b.Length == 0)) return a;
    
      int[] c = new int[a.Length + b.Length];
        
        for(int i = 0; i < (a.Length + b.Length); i++)
        {
            if(i< a.Length)
            c[i] = a[i];
            if(i>= a.Length)
            c[i] = b[i-a.Length];         
        }
    
    return c;

}
```
