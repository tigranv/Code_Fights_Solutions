```c#
int rectangleRotation(int a, int b) 
{
var x = (int) (a/Math.Sqrt(2));
var y = (int) (b/Math.Sqrt(2));
if ((x + y)%2 == 0) return x*y + (x + 1)*(y + 1);
return (x + 1)*y + (y + 1)*x;
}
```
