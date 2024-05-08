# integral-bases
Singular code and examples for computing integral bases and related staff

## Usage example:
```
LIB"integralbasis.lib";
ring r = 0, (x,y), dp;
poly f = (y4+3x3y + x4)*(y^7 + 6x4y3 + 2xy + x7)*(y5+7xy-4x2)*(y3+x2)*(y2-x3)+y30;
list l1 = integralBasis(f,2, "atOrigin", "opti1");  // Optimization by number of expansions in each class
list l2 = integralBasis(f,2, "atOrigin", "opti0");  // Classes are merged using Chinese remainder theorem
```
