```c#
int createAnagram(string s, string t)
{
    int count = s.Length;
    for (int i = 0; i < s.Length; i++)
    {
        for (int j = 0; j < t.Length; j++)
        {
            if (s[i] == t[j] )
            {
                count--;
                StringBuilder sb = new StringBuilder(t);
                sb[j] = '0';
                t = sb.ToString();
                break;
            }
        }
    }
    return count;
}
```
