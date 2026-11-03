# ⚙️ Methods

> Blocks of code that do a job: return types and the OpMode lifecycle methods init() and loop().

**4** items · **3** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Item | What it does |
|:--|:--|
| [`void`](#cmd-void) | Return type: the method does its job but gives no value back |
| [`return`](#cmd-return) | Sends a value back from a method that isn't void and ends it |
| [`init()`](#cmd-init) | Runs once when INIT is pressed; used to get the robot ready |
| [`loop()`](#cmd-loop) | Repeats about 50 times per second while the OpMode is running |

---

<a id="cmd-void"></a>

## `void`

Return type: the method does its job but gives no value back

```java
public void init() { }
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `int` | If the method returns a whole number, swap void for int and use return | `public int sumar() { return 5; }` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-return"></a>

## `return`

Sends a value back from a method that isn't void and ends it

```java
public int sumar() { return 5; }
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-init"></a>

## `init()`

Runs once when INIT is pressed; used to get the robot ready

```java
public void init() { telemetry.addData("Estado", "Listo"); }
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `( )` | The parentheses take the method's parameters; empty if it takes none | `public void init() { }` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-loop"></a>

## `loop()`

Repeats about 50 times per second while the OpMode is running

```java
public void loop() { telemetry.addData("Tiempo", getRuntime()); }
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(reading the gamepad)` | Read the controller inside loop() to see every change, about 50 times per second | `public void loop() { telemetry.addData("A", gamepad1.a); }` |

<sub>[⬆ Back to top](#commands)</sub>
