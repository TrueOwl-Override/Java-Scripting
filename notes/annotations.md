# 🏷️ Annotations

> Labels that start with @ and tell the compiler or the robot how to treat your code.

**4** items · **0** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Item | What it does |
|:--|:--|
| [`@ (annotation)`](#cmd-annotation) | Metadata that describes the code to the compiler or the system; it doesn't run anything |
| [`@Override`](#cmd-override) | Says you're replacing a method from the parent class; the compiler flags it if the name is misspelled |
| [`@TeleOp`](#cmd-teleop) | Registers the OpMode as a driver-controlled program so it shows up on the Driver Station |
| [`@Disabled`](#cmd-disabled) | Hides the OpMode from the Driver Station menu without deleting it (handy for tests) |

---

<a id="cmd-annotation"></a>

## `@ (annotation)`

Metadata that describes the code to the compiler or the system; it doesn't run anything

```java
@Override
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-override"></a>

## `@Override`

Says you're replacing a method from the parent class; the compiler flags it if the name is misspelled

```java
@Override public void init() { }
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-teleop"></a>

## `@TeleOp`

Registers the OpMode as a driver-controlled program so it shows up on the Driver Station

```java
@TeleOp
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-disabled"></a>

## `@Disabled`

Hides the OpMode from the Driver Station menu without deleting it (handy for tests)

```java
@Disabled
```

<sub>[⬆ Back to top](#commands)</sub>
