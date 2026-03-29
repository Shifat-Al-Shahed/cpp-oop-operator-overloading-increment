# cpp-oop-operator-overloading-increment
Simple C++ program to understand how ++ operator overloading works (pre and post increment).
```cpp
#include <bits/stdc++.h>
using namespace std;
class A
{
    int weight;
public:
    A(int weight = 0)
    {
        this->weight = weight;
    }

    void operator++()
    {
        ++weight;
    }
    void operator++(int)
    {
        weight++;
    }
    int get_weight();
};

int A ::get_weight()
{
    return weight;
}

signed main()
{
    int w; cin >> w;
    A shafi(w);
    ++shafi, shafi++;
    cout << "After pre increment and post increment his weight is : ";
    cout << shafi.get_weight() << '\n';
    return 0;
}

```
