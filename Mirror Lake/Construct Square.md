```c#
int constructSquare(string s)
{
    var f = getFreq(s);
    for (int i = 31622; i >= 0; --i) {
        if (E(f, getFreq(i * i + ""))) return i * i;
    }
    return -1;
}

bool E(int[] a, int[] b) {
    if (a.Length != b.Length) return false;
    for (int i = 0; i < a.Length; ++i) {
        if (a[i] != b[i]) {
            return false;
        }
    }
    return true;
}

int[] getFreq(string s) {
    var d = new Dictionary<char, int>();
    foreach (char c in s) {
        if (d.ContainsKey(c)) ++d[c];
        else d.Add(c, 1);
    }
    var ret = d.Values.ToArray();
    Array.Sort(ret);
    return ret;
}
```
