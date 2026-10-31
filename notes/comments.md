# 💬 Comments

> Notes for humans that the compiler skips: single-line, block and Javadoc comments.

**3** items · **1** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Item | What it does |
|:--|:--|
| [`//`](#cmd-sym-47-47) | Single-line comment: the compiler ignores everything after it on that line |
| [`/* */`](#cmd-sym-47-42-42-47) | Block comment: ignores everything between /* and */, even across several lines |
| [`/** */`](#cmd-sym-47-42-42-42-47) | Javadoc: a block comment that tools read to generate documentation and hover tooltips |

---

<a id="cmd-sym-47-47"></a>

## `//`

Single-line comment: the compiler ignores everything after it on that line

```java
double velocidad = 0.5; // potencia del motor (50 %)
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-sym-47-42-42-47"></a>

## `/* */`

Block comment: ignores everything between /* and */, even across several lines

```java
/* Espera 500 ms a que el sensor se estabilice */
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(nested)` | You can't put one /* */ inside another: the first */ closes the whole comment | `/* uno /* dos */` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-sym-47-42-42-42-47"></a>

## `/** */`

Javadoc: a block comment that tools read to generate documentation and hover tooltips

```java
/** Se ejecuta una vez al presionar INIT. */
```

<sub>[⬆ Back to top](#commands)</sub>
