# qa

`char` vs `unsigned char` vs `signed char`
***
```
char const * str_as_ptr1 = "123";
char const * str_as_ptr2 = "123";
``` 
vs 
```
char str_as_arr1[] = "123";
char str_as_arr2[] = "123";
```
***
```
void f1()
{
    std::array<long long, 2> p1;
    long long p2[2];
    long long * p3 = new long long [2];
}
```
vs
```
void f2()
{
    std::array<long long, 2> p1{};
    long long p2[2]{};
    long long * p3 = new long long [2]{};
}
```
***
`(i++ < 2) || (i == 3)` vs `(i++ < 2) + (i == 3)`
