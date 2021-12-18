#### 1. 预防空指针访问类成员变量   
```cpp
void showx()
{
    if (this == NULL)
    return;
    cout << "showx: " << x << endl;
}
```
