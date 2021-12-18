#### 1. 预防空指针访问类成员变量   
```cpp
void showx()
{
    if (this == NULL)
        return;
    cout << "showx: " << x << endl;
}
```  
#### 2. 静态变量作中介  
```cpp
static Person sp;
Person &operator+(Person &p1, Person &p2)
{
    sp._a = p1._a + p2._a;
    sp._b = p1._b + p2._b;
    return sp;
}
```
