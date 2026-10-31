# 🏗️ Program Structure

> How a Java file is put together: classes, access, inheritance, imports, braces and semicolons.

**11** items · **8** parameters  ·  [⬅ Back to index](../README.md)

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
| [`Case sensitivity`](#cmd-case-sensitivity) | Java tells upper and lower case apart: potencia and Potencia are different names; keywords are always lowercase |
| [`Whitespace`](#cmd-whitespace) | Java ignores spaces, tabs and line breaks; blocks are marked by braces, not indentation |
| [`( )`](#cmd-sym-40-41) | Every opening parenthesis needs a closing one; if one is missing, the program won't compile |

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
| `com.qualcomm.robotcore.eventloop.opmode.Autonomous` | Brings in the @Autonomous annotation | `import com.qualcomm.robotcore.eventloop.opmode.Autonomous;` |

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

| Parameter | What it does | Example |
|:--|:--|:--|
| `(after })` | No semicolon after a closing brace | `public void loop() { }` |
| `(in comments)` | Inside a comment the ; is ignored like everything else | `// x = 5;` |

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

---

<a id="cmd-case-sensitivity"></a>

## `Case sensitivity`

Java tells upper and lower case apart: potencia and Potencia are different names; keywords are always lowercase

```java
int potencia = 1; // Potencia would fail: it doesn't exist
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-whitespace"></a>

## `Whitespace`

Java ignores spaces, tabs and line breaks; blocks are marked by braces, not indentation

```java
int a = 1; int b = 2;
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-sym-40-41"></a>

## `( )`

Every opening parenthesis needs a closing one; if one is missing, the program won't compile

```java
telemetry.addData("Nombre", "Ashton");
```

<sub>[⬆ Back to top](#commands)</sub>
