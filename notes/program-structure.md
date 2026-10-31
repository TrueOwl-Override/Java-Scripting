# 🏗️ Program Structure

> How a Java file is put together: classes, access, inheritance, imports, braces and semicolons.

**8** items · **5** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Item | What it does |
|:--|:--|
| [`class`](#cmd-class) | Defines a class: the container where all Java code lives |
| [`public`](#cmd-public) | Access modifier: lets other classes and the robot's system use the class or method |
| [`extends`](#cmd-extends) | Inheritance: the child class gets everything the parent class already has |
| [`import`](#cmd-import) | Brings in a class from a library (like the FTC SDK) so you can use it in the file |
| [`{ }`](#cmd-sym-123-125) | Braces: mark where a class or method starts and ends; they always come in pairs |
| [`;`](#cmd-sym-59) | Ends every statement; lines that open a brace { don't take one |
| [`PascalCase`](#cmd-pascalcase) | Naming convention for classes: every word starts with a capital letter |
| [`File name = class name`](#cmd-file-name-class-name) | A public class must have the same name as its .java file, capital letters included |

---

<a id="cmd-class"></a>

## `class`

Defines a class: the container where all Java code lives

```java
public class HelloWorld extends OpMode { }
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-public"></a>

## `public`

Access modifier: lets other classes and the robot's system use the class or method

```java
public void init() { }
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `(no public)` | Access only inside the same package; the robot's system couldn't load the OpMode | `class Prueba { }` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-extends"></a>

## `extends`

Inheritance: the child class gets everything the parent class already has

```java
public class HelloWorld extends OpMode { }
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `OpMode` | FTC SDK base class: gives you init(), loop(), telemetry and hardware access | `public class HelloWorld extends OpMode { }` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-import"></a>

## `import`

Brings in a class from a library (like the FTC SDK) so you can use it in the file

```java
import com.qualcomm.robotcore.eventloop.opmode.OpMode;
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `com.qualcomm.robotcore.eventloop.opmode.OpMode` | Brings in the OpMode class from the FTC SDK | `import com.qualcomm.robotcore.eventloop.opmode.OpMode;` |
| `com.qualcomm.robotcore.eventloop.opmode.TeleOp` | Brings in the @TeleOp annotation | `import com.qualcomm.robotcore.eventloop.opmode.TeleOp;` |
| `com.qualcomm.robotcore.eventloop.opmode.Disabled` | Brings in the @Disabled annotation | `import com.qualcomm.robotcore.eventloop.opmode.Disabled;` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-sym-123-125"></a>

## `{ }`

Braces: mark where a class or method starts and ends; they always come in pairs

```java
public void loop() { }
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-sym-59"></a>

## `;`

Ends every statement; lines that open a brace { don't take one

```java
String saludo = "Hola";
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-pascalcase"></a>

## `PascalCase`

Naming convention for classes: every word starts with a capital letter

```java
public class SensorColor { }
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-file-name-class-name"></a>

## `File name = class name`

A public class must have the same name as its .java file, capital letters included

```java
HelloWorld.java → public class HelloWorld { }
```

<sub>[⬆ Back to top](#commands)</sub>
