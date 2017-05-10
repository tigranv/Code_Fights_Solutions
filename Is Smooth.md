```c#
bool isSmooth(int[] arr) {
   
    
    if (arr[0] == arr[arr.Length-1])
            {
                if (arr.Length%2 == 0)
                {
                    return (arr[0] == (arr[arr.Length / 2] + arr[arr.Length / 2 - 1])) ? true : false;
                }
                else
                {
                     return (arr[0] == arr[arr.Length / 2]) ? true : false;
                }

            }
           
 return false;
}
```
