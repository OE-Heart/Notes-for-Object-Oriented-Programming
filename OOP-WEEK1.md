# WEEK 1

## The C language

### Strengths

- Efficient programs
- Direct access to machine, suitable for OS and ES
- Flexible

### Weakness

- Insufficient type checking
- Poor support for programming-in-the-large
- Procedure-oriented programming

## C++ improvements

- Data abstraction
- Access control
- Initialization & cleanup
- Function overloading
- Streams for I/O
- Constants (C99)
- Name control
- Inline functions(C99)
- References
- Operator overloading
- Memory management
- Support for OOP
- Templates
- Exception handling
- Extensive libraries, STL

## The string class

```c++
#include <string> //must add this at the head of code
```

- Define variable of string like other types

  ```c++
  string str;
  ```

- Initialize with string content

  ```c++
  string str = "Hello";
  ```

- Read and write string with cin/cout

  ```c++
  cin >> str;
  cout << str;
  ```

### Concatenation for string

```c++
string str3;
str3 = str1 + str2;
str1 += str2;
str1 += "lalala";
```

### Ctors

```c++
string (const char *cp, int len);
string (const string& s2, int pos);
string (const string& s2, int pos, int len);
```

### Sub-string

```c++
substr (int pos, int len);
```

### Alter string

```c++
assign (…);
insert (…);
insert (int pos, const string& s);
erase (…);
append (…);
replace (int pos, int len, const string& s);
```

### Search string

```c++
find (const string& s);
```

## File I/O

```c++
#include <ifstream>  // read from file
#include <ofstream>  // write to file
```

```c++
ofstream File1("C:\\test.txt");
File1 << "Hello world" << std::endl;
```

```c++
ifstream File2("C:\\test.txt");
std::string str;
File2 >> str;
```