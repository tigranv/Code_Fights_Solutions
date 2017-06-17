```c#
int comfortableNumbers(int L, int R)
{
    if(L==R)
        return 0;
 
    int a = L, b = a + 1, sumA = 0, pairs = 0;
    List<string> listPairs = new List<string>();
    while (a < R) 
    {
        string aStr = a.ToString();
        int aX = 0;
 
        while (aX < aStr.Length) 
        {
            sumA = sumA + int.Parse(aStr[aX]+"");
            aX = aX + 1;
        }
        while (b <= R) 
        {
            string bStr = b.ToString();
            int bX = 0, sumB = 0;
 
            while (bX < bStr.Length) 
            {
                sumB = sumB + int.Parse(bStr[bX]+"");
                bX = bX + 1;
            }
 
            if((b >= a - sumA) && (b <= a + sumA)&&
              (a >= b - sumB) && (a <= b + sumB)) 
              {
                pairs = pairs + 1;
              }
 
            b ++;
        }
 
        a = a + 1;
        b = a + 1;
        sumA = 0;
    }
    return pairs;
}
```
