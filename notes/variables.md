# 📦 Variables

> Named boxes in memory: how to name, declare, assign and initialize them.

**7** items · **2** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Item | What it does |
|:--|:--|
| [`Variable`](#cmd-variable) | A named spot in memory that holds a value; its size depends on its type |
| [`camelCase`](#cmd-camelcase) | Naming convention for variables: start lowercase, every next word starts with a capital |
| [`Declaration`](#cmd-declaration) | type name; reserves the space with a type and a name; required before using the variable |
| [`= (assignment)`](#cmd-assignment) | Stores the value on the right in the variable on the left; it doesn't mean equality |
| [`Reassignment`](#cmd-reassignment) | A variable can get new values many times; it always keeps the latest and the old one is lost |
| [`Initialization`](#cmd-initialization) | type name = value; declares and assigns in one line; the most common way |
| [`Default values`](#cmd-default-values) | Class fields with no value start at 0 (numbers) or false (boolean); a local variable must be assigned before it is read |

---

<a id="cmd-variable"></a>

## `Variable`

A named spot in memory that holds a value; its size depends on its type

```java
int teamNumber;
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-camelcase"></a>

## `camelCase`

Naming convention for variables: start lowercase, every next word starts with a capital

```java
double motorSpeed = 0.5;
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-declaration"></a>

## `Declaration`

type name; reserves the space with a type and a name; required before using the variable

```java
int teamNumber;
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-assignment"></a>

## `= (assignment)`

Stores the value on the right in the variable on the left; it doesn't mean equality

```java
teamNumber = 16072;
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(value on the left)` | The left side must always be a variable: 10 = x; won't compile | `int x = 10; // 10 = x; no compila` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-reassignment"></a>

## `Reassignment`

A variable can get new values many times; it always keeps the latest and the old one is lost

```java
int x = 5; x = 10; // x vale 10
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-initialization"></a>

## `Initialization`

type name = value; declares and assigns in one line; the most common way

```java
double motorSpeed = 0.5;
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-default-values"></a>

## `Default values`

Class fields with no value start at 0 (numbers) or false (boolean); a local variable must be assigned before it is read

```java
public class Robot { int vueltas; boolean listo; }
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(local variable)` | Inside a method there is no default: assign it before using it | `int vueltas = 0;` |

<sub>[⬆ Back to top](#commands)</sub>
