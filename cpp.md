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
#### 3. 指针强行访问私有属性  
```cpp
class A
{
private:
    int _x = 0;
};

int main()
{
    A a;
    int *p = (*int)&a;
    cout << *p << endl;
}
```  
#### 4. 指针在类间强转  
```cpp
class A
{
public:
    A() { cout << "A" << endl; }
    void show_a()
    {
        cout << _a << endl;
    }

private:
    bool _a = 1;
};

class B
{
public:
    B() { cout << "B" << endl; }
    int _b = 255;
};

void test01()
{
    B b;
    B *p = &b;
    cout << p << endl
         << ((A *)p) << endl;
    ((A *)p)->show_a();
}
```  
> 输出结果为20，由于将指针强转为A*，例子中调用show_a()函数需要访问_a这个bool型变量，于是编译器在b的内存处向后访问1字节，即_b，得到255这个结果，如果_b=256，那么show_a()调用输出的结果就为0。若A类中_a的类型为double，即大于_b的int，那么调用show_a()会访问8字节，超过_b的储存区域。
