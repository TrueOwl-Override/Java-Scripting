# 🔤 Strings & Types

> Working with text and data types.

**15** items · **8** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Item | What it does |
|:--|:--|
| [`.equals()`](#cmd-equals) | Compares the text of two Strings; == only checks whether they are the same object |
| [`Primitive types`](#cmd-primitive-types) | Java's 8 built-in types: byte, short, int, long, float, double, char and boolean; FTC mostly uses int, double and boolean |
| [`byte`](#cmd-byte) | 8-bit whole number: from -128 to 127 |
| [`short`](#cmd-short) | 16-bit whole number (-32,768 to 32,767); almost never used in FTC |
| [`char`](#cmd-char) | A single Unicode character, in single quotes |
| [`int`](#cmd-int) | 32-bit whole number (-2,147,483,648 to 2,147,483,647); the standard for counting |
| [`long`](#cmd-long) | 64-bit whole number (up to ~9 quintillion); use it when an int isn't big enough |
| [`float`](#cmd-float) | 32-bit decimal (~7 digits of precision); smaller than a double |
| [`double`](#cmd-double) | 64-bit decimal (~15-17 digits); Java's default decimal type and what sensors return |
| [`boolean`](#cmd-boolean) | Holds only true or false; it doesn't accept 1 or 0 and can't be added |
| [`true / false`](#cmd-true-false) | Java's logical values; always lowercase (True won't compile) |
| [`String`](#cmd-string) | Class for holding text; written with a capital S and the value goes in double quotes |
| [`" " (double quotes)`](#cmd-double-quotes) | Wrap a text (String); single quotes ' ' are only for a char |
| [`Class vs. primitive`](#cmd-class-vs-primitive) | Primitives (int, double) are lowercase; String is a class, so it starts with a capital letter |
| [`Concatenation (+)`](#cmd-concatenation) | Joins texts, or text with numbers, into one String; it doesn't add spaces on its own |

---

<a id="cmd-equals"></a>

## `.equals()`

Compares the text of two Strings; == only checks whether they are the same object

```java
String a = "hola"; boolean igual = a.equals("hola");
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-primitive-types"></a>

## `Primitive types`

Java's 8 built-in types: byte, short, int, long, float, double, char and boolean; FTC mostly uses int, double and boolean

```java
int a = 1; double b = 0.5; boolean c = true;
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-byte"></a>

## `byte`

8-bit whole number: from -128 to 127

```java
byte nivel = 100;
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-short"></a>

## `short`

16-bit whole number (-32,768 to 32,767); almost never used in FTC

```java
short temperatura = 1200;
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-char"></a>

## `char`

A single Unicode character, in single quotes

```java
char letra = 'A';
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-int"></a>

## `int`

32-bit whole number (-2,147,483,648 to 2,147,483,647); the standard for counting

```java
int teamNumber = 16072;
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(with decimals)` | An int can't hold decimals: int x = 0.5; is an error, use double | `double x = 0.5; // int x = 0.5; no compila` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-long"></a>

## `long`

64-bit whole number (up to ~9 quintillion); use it when an int isn't big enough

```java
long granos = 3000000000L;
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `L (suffix)` | A number too big for an int needs an L at the end; without it, it won't compile | `long granos = 3000000000L;` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-float"></a>

## `float`

32-bit decimal (~7 digits of precision); smaller than a double

```java
float pi = 3.14f;
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `f (suffix)` | Without the f, 3.14 is treated as a double and won't compile | `float pi = 3.14f;` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-double"></a>

## `double`

64-bit decimal (~15-17 digits); Java's default decimal type and what sensors return

```java
double motorSpeed = 0.5;
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-boolean"></a>

## `boolean`

Holds only true or false; it doesn't accept 1 or 0 and can't be added

```java
boolean touchSensorPressed = true;
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(with 1 / 0)` | Java doesn't turn numbers into booleans: boolean b = 1; is an error | `boolean b = true; // boolean b = 1; no compila` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-true-false"></a>

## `true / false`

Java's logical values; always lowercase (True won't compile)

```java
boolean esRojo = true;
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-string"></a>

## `String`

Class for holding text; written with a capital S and the value goes in double quotes

```java
String myName = "Alan Smith";
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(with single quotes)` | A text in ' ' won't compile: single quotes are only for a char | `String nombre = "Alan"; // String nombre = 'Alan'; no compila` |
| `(lowercase s)` | string doesn't exist in Java: you get a cannot find symbol error | `String ok = "sí"; // string mal = "no"; no compila` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-double-quotes"></a>

## `" " (double quotes)`

Wrap a text (String); single quotes ' ' are only for a char

```java
String nombre = "Ashton"; char inicial = 'A';
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-class-vs-primitive"></a>

## `Class vs. primitive`

Primitives (int, double) are lowercase; String is a class, so it starts with a capital letter

```java
int x = 5; String texto = "cinco";
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-concatenation"></a>

## `Concatenation (+)`

Joins texts, or text with numbers, into one String; it doesn't add spaces on its own

```java
String saludo = "Hola, " + myName;
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(no space)` | If you don't put the space inside the quotes, the text comes out stuck together | `String pegado = "Hola" + "Alan"; // "HolaAlan"` |
| `(with a number)` | If one side is a String, Java turns the number into text automatically | `String equipo = "Equipo: " + 16072; // "Equipo: 16072"` |

<sub>[⬆ Back to top](#commands)</sub>
