```c#
bool willYou(bool young, bool beautiful, bool loved) 
{
    if ((young && beautiful && !loved) || (loved && (!young || !beautiful)))  return true;
    
    return false;
}
```
