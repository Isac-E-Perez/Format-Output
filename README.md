# Format Output
## About

The C++ escape sequences are pretty similar to other languages. The most common ones are: \n - newline \t - tab. We can also format the output by using the iomanip library like I did below.

```c++
/*
Escape Sequences:
\n : newline
\t : tab
*/
#include <iostream> 
#include <iomanip> // iomanip library for formatting output
using namespace std;

 int main()
 {
     int a = 45;
     float b = 45.323;
     double c = 45.5468;
     int aa = a + 9;
     float bb = b + 9;
     double cc = c + 9;
     int aaa = aa + 9;
     float bbb = bb + 9;
     double ccc = cc + 9;

     cout << "print with set width = 10\n"; // setw : set width 
     cout << "Ints"<< setw(10) << "Floats" << setw(10) << "Doubles" << setw(10) << "\n";

     cout << a << setw(12) << b << setw(10)<< c << "\n";    

     cout << aa << setw(12)<< bb << setw(10)<< cc << "\n";  

     cout << aaa << setw(12)<< bbb << setw(10)<< ccc << "\n\n"; 

     cout << "print with tabs\n";
     cout << "Int" << "\tFloats" << "\tDoubles\n";
     cout << aaa << "\t" << bbb << "\t" << ccc << "\n"; 

     return 0;
 }
```
The output we get is:
```c++
print with set width = 10
Ints    Floats   Doubles         
45      45.323   45.5468
54      54.323   54.5468
63      63.323   63.5468

print with tabs
Int     Floats  Doubles
63      63.323  63.5468
```
