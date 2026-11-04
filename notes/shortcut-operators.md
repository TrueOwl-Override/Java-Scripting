# 🔁 Shortcut Operators

> Update a variable without repeating its name: ++, -- and compound assignment (+=, -=, *=, /=, %=).

**8** items · **5** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Item | What it does |
|:--|:--|
| [`Compound assignment`](#cmd-compound-assignment) | Does the operation and stores the result in the same variable, without repeating its name |
| [`++ (increment)`](#cmd-increment) | Adds 1 to the variable; same as x = x + 1 |
| [`-- (decrement)`](#cmd-decrement) | Subtracts 1 from the variable; same as x = x - 1 |
| [`+= (add and assign)`](#cmd-add-and-assign) | Adds a value and stores it in the same variable; same as x = x + n |
| [`-= (subtract and assign)`](#cmd-subtract-and-assign) | Subtracts a value and stores it in the same variable; same as x = x - n |
| [`*= (multiply and assign)`](#cmd-multiply-and-assign) | Multiplies and stores in the same variable; handy for scaling values |
| [`/= (divide and assign)`](#cmd-divide-and-assign) | Divides and stores in the same variable; with int it truncates too |
| [`%= (remainder and assign)`](#cmd-remainder-and-assign) | Stores in the variable the remainder of dividing it |

---

<a id="cmd-compound-assignment"></a>

## `Compound assignment`

Does the operation and stores the result in the same variable, without repeating its name

```java
double velocidad = 0.5; velocidad *= 2; // 1.0
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-increment"></a>

## `++ (increment)`

Adds 1 to the variable; same as x = x + 1

```java
int x = 5; x++; // 6
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(counter)` | Used to count how many times something happens | `int vueltas = 0; vueltas++; // 1` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-decrement"></a>

## `-- (decrement)`

Subtracts 1 from the variable; same as x = x - 1

```java
int intentos = 3; intentos--; intentos--; // 1
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-add-and-assign"></a>

## `+= (add and assign)`

Adds a value and stores it in the same variable; same as x = x + n

```java
int puntos = 0; puntos += 50; // 50
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-subtract-and-assign"></a>

## `-= (subtract and assign)`

Subtracts a value and stores it in the same variable; same as x = x - n

```java
int puntos = 150; puntos -= 50; // 100
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(vs. -)` | -= changes the variable; - only calculates a new result. To show a subtraction in telemetry, use - | `telemetry.addData("Resta de sticks", gamepad1.left_stick_y - gamepad1.right_stick_y);` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-multiply-and-assign"></a>

## `*= (multiply and assign)`

Multiplies and stores in the same variable; handy for scaling values

```java
int velocidad = 10; velocidad *= 3; // 30
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(with double)` | Scales a power value without losing decimals | `double potencia = 0.8; potencia *= 0.5; // 0.4` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-divide-and-assign"></a>

## `/= (divide and assign)`

Divides and stores in the same variable; with int it truncates too

```java
int galletas = 10; galletas /= 2; // 5
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(with int)` | If the variable is an int, the decimal part is thrown away | `int x = 7; x /= 2; // 3` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-remainder-and-assign"></a>

## `%= (remainder and assign)`

Stores in the variable the remainder of dividing it

```java
int segundos = 125; segundos %= 60; // 5
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(circular range)` | Keeps a value inside a range that starts over | `int paso = 5; paso %= 4; // 1` |

<sub>[⬆ Back to top](#commands)</sub>
