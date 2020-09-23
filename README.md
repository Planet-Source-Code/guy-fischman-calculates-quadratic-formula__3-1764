<div align="center">

## Calculates Quadratic Formula


</div>

### Description

This code applies the quadratic formula to an equation and derives the variable value given the three coefficients.
 
### More Info
 
Three coefficients of a quadratic equation.

Value of unknown variable.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Guy Fischman](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/guy-fischman.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |C, C\+\+ \(general\)
**Category**       |[Math](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/math__3-12.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/guy-fischman-calculates-quadratic-formula__3-1764/archive/master.zip)

### API Declarations

```
iostream.h
math.h
```


### Source Code

```
#include <iostream.h>
#include <math.h>
void main()
{
 double A;
 double B;
 double C;
 double disc;
 cout << "Enter A: ";
 cin >> A;
 cout << "Enter B: ";
 cin >> B;
 cout << "Enter C: ";
 cin >> C;
 disc = B*B - 4*A*C;
 if (disc < 0){
 cout << "Imaginary results: " << endl;
 cout << "(" << B * (-1) << " + " << sqrt(disc * (-1)) << "i) / " << 2*A << endl;
 cout << "(" << B * (-1) << " - " << sqrt(disc * (-1)) << "i) / " << 2*A << endl;
 }
 else if (disc == 0){
 cout << "Single result: " << (-B)/(2*A) << endl;
 }
 else{
  cout << "Two results: " << endl;
  cout << (B * (-1) + sqrt(disc)) / (2*A) << endl;
  cout << (B * (-1) - sqrt(disc)) / (2*A) << endl;
 }
}
```

