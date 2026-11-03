# ➗ Math Operators

> Do math with numbers: arithmetic, negation, integer division, modulo and order of operations.

**9** items · **8** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Item | What it does |
|:--|:--|
| [`+ (addition)`](#cmd-addition) | Adds two numbers |
| [`- (subtraction)`](#cmd-subtraction) | Subtracts the number on the right from the one on the left |
| [`- (negation)`](#cmd-negation) | Unary operator: flips the sign of a single value |
| [`* (multiplication)`](#cmd-multiplication) | Multiplies; the symbol is always required |
| [`/ (division)`](#cmd-division) | Divides; if both numbers are int, the result is an int too |
| [`Truncation (int / int)`](#cmd-truncation-int-int) | int / int throws away the decimal part; it doesn't round |
| [`% (modulo)`](#cmd-modulo) | Gives the remainder (what's left over) of a whole-number division |
| [`Order of operations`](#cmd-order-of-operations) | * / % are solved before + -; ties go left to right |
| [`( ) (precedence)`](#cmd-precedence) | Whatever is inside parentheses is calculated first |

---

<a id="cmd-addition"></a>

## `+ (addition)`

Adds two numbers

```java
int total = 3 + 4; // 7
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-subtraction"></a>

## `- (subtraction)`

Subtracts the number on the right from the one on the left

```java
double diferencia = 1.0 - 0.25; // 0.75
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-negation"></a>

## `- (negation)`

Unary operator: flips the sign of a single value

```java
double avance = -gamepad1.left_stick_y;
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(0 - x)` | -x is the same as 0 - x | `double x = 0.8; double y = 0 - x; // -0.8` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-multiplication"></a>

## `* (multiplication)`

Multiplies; the symbol is always required

```java
double potencia = 0.8 * 0.5; // 0.4
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(no symbol)` | You can't put numbers side by side: 3x isn't valid, write 3 * x | `int x = 4; int y = 3 * x; // 12` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-division"></a>

## `/ (division)`

Divides; if both numbers are int, the result is an int too

```java
double mitad = 1.0 / 2; // 0.5
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(with a decimal)` | One number with a decimal point is enough to avoid truncation | `double r = 5.0 / 2; // 2.5` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-truncation-int-int"></a>

## `Truncation (int / int)`

int / int throws away the decimal part; it doesn't round

```java
int r = 5 / 2; // 2
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(result 0)` | If the divisor is bigger, int / int gives 0 | `int r = 9 / 10; // 0` |
| `(stopped motor)` | A power calculated with int / int can be 0 and leave the robot still | `double potencia = 1 / 2; // 0.0, usa 1.0 / 2` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-modulo"></a>

## `% (modulo)`

Gives the remainder (what's left over) of a whole-number division

```java
int resto = 11 % 4; // 3
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(n % 2 == 0)` | Tells you whether a number is even | `boolean esPar = 8 % 2 == 0; // true` |
| `(cyclic counter)` | Makes a counter go back to 0 when it reaches a limit | `int paso = 3; paso = (paso + 1) % 4; // vuelve a 0` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-order-of-operations"></a>

## `Order of operations`

* / % are solved before + -; ties go left to right

```java
int r = 10 + 5 * 2; // 20
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-precedence"></a>

## `( ) (precedence)`

Whatever is inside parentheses is calculated first

```java
int r = 3 * (4 + 2); // 18
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(for readability)` | Use them even when they aren't needed so the formula is easy to read | `double v = (-gamepad1.left_stick_y) / 2.0;` |

<sub>[⬆ Back to top](#commands)</sub>
