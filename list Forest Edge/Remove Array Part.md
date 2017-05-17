```c#
int[] removeArrayPart(int[] inputArray, int l, int r)
        {
            if(inputArray.Length == 0) return inputArray;
            int[] newarr = new int[inputArray.Length - (r-l+1)];

            for (int i = 0; i < newarr.Length; i++)
            {
                if (i<l)
                {
                    newarr[i] = inputArray[i];
                }
                if (i >=l)
                {
                    newarr[i] = inputArray[i+ (r - l + 1)];
                }
            }
          
            return newarr;
            
        }
        ```
