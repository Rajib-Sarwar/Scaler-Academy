# Advanced DSA : Maths - GCD

**GCD** = Greatest Common Divisor or **HCF** = Highest Common Factor

**LCM** = Least Common Multiple

## Relation between GCD and LCM (Important)

Suppose, A & B are real numbers,

**A * B = GCD(A, B) * LCM(A,B)**


### Example:
```
A = 75 & B = 100
A * B = 7500

GCD(75, 100) = 25
LCM(75, 100) = 300
GCD(A, B) * LCM(A,B) = 7500 

so, A * B = GCD(A, B) * LCM(A,B)
```

### Properties
```
1. gcd(a, b) = gcd(|a|, |b|)
2. gcd(a, b) = gcd(b, a) [ Communtative property ]
3. gcd(a, 0) = a
4. gcd(a, 1) = 1
5. gcd(a, b, c) = gc(a, gcd(b,c))  [ Assotiative Properties ]
                = gc(b, gcd(a,c))
                = gc(c, gcd(b,c))
```

## Euclidean Algorithm for finding GCD

```
int gcd(int A, int B) {
    if(B == 0) return A;
    return gcd(B, A%B);
}
```
