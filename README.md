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
`char * ptr = new char [3];` vs `char ptr[3];` vs `std::array<char, 3> ptr;`
