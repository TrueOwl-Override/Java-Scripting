# 🔭 Scope

> Where a variable lives: blocks, braces and which code can see each variable.

**3** items · **1** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Item | What it does |
|:--|:--|
| [`Scope`](#cmd-scope) | Where a variable exists: it's born at its declaration and dies at the } of the block where it was created |
| [`Block`](#cmd-block) | Any section of code between { and }; each block has its own scope |
| [`Block hierarchy`](#cmd-block-hierarchy) | Variables from an outer block are visible in inner blocks, but not the other way around |

---

<a id="cmd-scope"></a>

## `Scope`

Where a variable exists: it's born at its declaration and dies at the } of the block where it was created

```java
int x = 5; { int y = 4; x = x + y; } // aquí y ya no existe
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(outside the block)` | Using a variable after its } gives a cannot find symbol error | `int x = 5; { int y = 4; } x = 10; // x = y; no compila` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-block"></a>

## `Block`

Any section of code between { and }; each block has its own scope

```java
{ int y = 4; }
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-block-hierarchy"></a>

## `Block hierarchy`

Variables from an outer block are visible in inner blocks, but not the other way around

```java
int x = 5; { int y = x + 1; }
```

<sub>[⬆ Back to top](#commands)</sub>
