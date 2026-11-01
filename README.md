<div align="center">

# ☕ Java Scripting

**A personal reference for learning Java (with FTC robotics in mind): keywords, syntax and concepts, with examples that compile.**

![Concepts](https://img.shields.io/badge/concepts-42-2ea44f?style=for-the-badge) ![Parameters](https://img.shields.io/badge/parameters-18-0969da?style=for-the-badge) ![Categories](https://img.shields.io/badge/categories-7-8250df?style=for-the-badge)

🌐 **Searchable web version:** [`docs/index.html`](docs/index.html)  ·  🐧 **Companion repos:** [Linux-Commands](https://github.com/TrueOwl-Override/Linux-Commands) · [Bash-Scripting-From-Scratch](https://github.com/TrueOwl-Override/Bash-Scripting-From-Scratch)

</div>

---

## 📚 Categories

| | Category | What's inside | Items |
|:-:|:--|:--|:--|
| 🏗️ | **[Program Structure](notes/program-structure.md)** | How a Java file is put together: classes, access, inheritance, imports, braces and semicolons. | `class` `public` `extends` `import` `{ }` `;` `PascalCase` `File name = class name` `Case sensitivity` `Whitespace` `( )` |
| 💬 | **[Comments](notes/comments.md)** | Notes for humans that the compiler skips: single-line, block and Javadoc comments. | `//` `/* */` `/** */` |
| 🏷️ | **[Annotations](notes/annotations.md)** | Labels that start with @ and tell the compiler or the robot how to treat your code. | `@ (annotation)` `@Override` `@TeleOp` `@Disabled` `@Autonomous` |
| ⚙️ | **[Methods](notes/methods.md)** | Blocks of code that do a job: return types and the OpMode lifecycle methods init() and loop(). | `void` `return` `init()` `loop()` |
| 📡 | **[Telemetry](notes/telemetry.md)** | Send data from the robot to the Driver Station screen to see what it's doing. | `telemetry.addData()` |
| 📦 | **[Variables](notes/variables.md)** | Named boxes in memory: how to name, declare, assign and initialize them. | `Variable` `camelCase` `Declaration` `= (assignment)` `Reassignment` `Initialization` `Default values` |
| 🔤 | **[Strings & Types](notes/strings-types.md)** | Working with text and data types. | `.equals()` `Primitive types` `byte` `short` `char` `int` `long` `float` `double` `boolean` `true / false` |

## 🔤 A–Z index

| Item | What it does | Category |
|:--|:--|:--|
| [`boolean`](notes/strings-types.md#cmd-boolean) | Holds only true or false; it doesn't accept 1 or 0 and can't be added | 🔤 Strings & Types |
| [`byte`](notes/strings-types.md#cmd-byte) | 8-bit whole number: from -128 to 127 | 🔤 Strings & Types |
| [`camelCase`](notes/variables.md#cmd-camelcase) | Naming convention for variables: start lowercase, every next word starts with a capital | 📦 Variables |
| [`Case sensitivity`](notes/program-structure.md#cmd-case-sensitivity) | Java tells upper and lower case apart: potencia and Potencia are different names; keywords are always lowercase | 🏗️ Program Structure |
| [`char`](notes/strings-types.md#cmd-char) | A single Unicode character, in single quotes | 🔤 Strings & Types |
| [`class`](notes/program-structure.md#cmd-class) | Defines a class: the container where all Java code lives | 🏗️ Program Structure |
| [`Declaration`](notes/variables.md#cmd-declaration) | type name; reserves the space with a type and a name; required before using the variable | 📦 Variables |
| [`Default values`](notes/variables.md#cmd-default-values) | Class fields with no value start at 0 (numbers) or false (boolean); a local variable must be assigned before it is read | 📦 Variables |
| [`double`](notes/strings-types.md#cmd-double) | 64-bit decimal (~15-17 digits); Java's default decimal type and what sensors return | 🔤 Strings & Types |
| [`extends`](notes/program-structure.md#cmd-extends) | Inheritance: the child class gets everything the parent class already has | 🏗️ Program Structure |
| [`File name = class name`](notes/program-structure.md#cmd-file-name-class-name) | A public class must have the same name as its .java file, capital letters included | 🏗️ Program Structure |
| [`float`](notes/strings-types.md#cmd-float) | 32-bit decimal (~7 digits of precision); smaller than a double | 🔤 Strings & Types |
| [`import`](notes/program-structure.md#cmd-import) | Brings in a class from a library (like the FTC SDK) so you can use it in the file | 🏗️ Program Structure |
| [`init()`](notes/methods.md#cmd-init) | Runs once when INIT is pressed; used to get the robot ready | ⚙️ Methods |
| [`Initialization`](notes/variables.md#cmd-initialization) | type name = value; declares and assigns in one line; the most common way | 📦 Variables |
| [`int`](notes/strings-types.md#cmd-int) | 32-bit whole number (-2,147,483,648 to 2,147,483,647); the standard for counting | 🔤 Strings & Types |
| [`long`](notes/strings-types.md#cmd-long) | 64-bit whole number (up to ~9 quintillion); use it when an int isn't big enough | 🔤 Strings & Types |
| [`loop()`](notes/methods.md#cmd-loop) | Repeats about 50 times per second while the OpMode is running | ⚙️ Methods |
| [`PascalCase`](notes/program-structure.md#cmd-pascalcase) | Naming convention for classes: every word starts with a capital letter | 🏗️ Program Structure |
| [`Primitive types`](notes/strings-types.md#cmd-primitive-types) | Java's 8 built-in types: byte, short, int, long, float, double, char and boolean; FTC mostly uses int, double and boolean | 🔤 Strings & Types |
| [`public`](notes/program-structure.md#cmd-public) | Access modifier: lets other classes and the robot's system use the class or method | 🏗️ Program Structure |
| [`Reassignment`](notes/variables.md#cmd-reassignment) | A variable can get new values many times; it always keeps the latest and the old one is lost | 📦 Variables |
| [`return`](notes/methods.md#cmd-return) | Sends a value back from a method that isn't void and ends it | ⚙️ Methods |
| [`short`](notes/strings-types.md#cmd-short) | 16-bit whole number (-32,768 to 32,767); almost never used in FTC | 🔤 Strings & Types |
| [`telemetry.addData()`](notes/telemetry.md#cmd-telemetry-adddata) | Sends a label and a value to the Driver Station screen for debugging | 📡 Telemetry |
| [`true / false`](notes/strings-types.md#cmd-true-false) | Java's logical values; always lowercase (True won't compile) | 🔤 Strings & Types |
| [`Variable`](notes/variables.md#cmd-variable) | A named spot in memory that holds a value; its size depends on its type | 📦 Variables |
| [`void`](notes/methods.md#cmd-void) | Return type: the method does its job but gives no value back | ⚙️ Methods |
| [`Whitespace`](notes/program-structure.md#cmd-whitespace) | Java ignores spaces, tabs and line breaks; blocks are marked by braces, not indentation | 🏗️ Program Structure |
| [`( )`](notes/program-structure.md#cmd-sym-40-41) | Every opening parenthesis needs a closing one; if one is missing, the program won't compile | 🏗️ Program Structure |
| [`.equals()`](notes/strings-types.md#cmd-equals) | Compares the text of two Strings; == only checks whether they are the same object | 🔤 Strings & Types |
| [`/* */`](notes/comments.md#cmd-sym-47-42-42-47) | Block comment: ignores everything between /* and */, even across several lines | 💬 Comments |
| [`/** */`](notes/comments.md#cmd-sym-47-42-42-42-47) | Javadoc: a block comment that tools read to generate documentation and hover tooltips | 💬 Comments |
| [`//`](notes/comments.md#cmd-sym-47-47) | Single-line comment: the compiler ignores everything after it on that line | 💬 Comments |
| [`;`](notes/program-structure.md#cmd-sym-59) | Ends every statement; lines that open a brace { don't take one | 🏗️ Program Structure |
| [`= (assignment)`](notes/variables.md#cmd-assignment) | Stores the value on the right in the variable on the left; it doesn't mean equality | 📦 Variables |
| [`@ (annotation)`](notes/annotations.md#cmd-annotation) | Metadata that describes the code to the compiler or the system; it doesn't run anything | 🏷️ Annotations |
| [`@Autonomous`](notes/annotations.md#cmd-autonomous) | Registers the OpMode in the Driver Station's Autonomous list instead of TeleOp | 🏷️ Annotations |
| [`@Disabled`](notes/annotations.md#cmd-disabled) | Hides the OpMode from the Driver Station menu without deleting it (handy for tests) | 🏷️ Annotations |
| [`@Override`](notes/annotations.md#cmd-override) | Says you're replacing a method from the parent class; the compiler flags it if the name is misspelled | 🏷️ Annotations |
| [`@TeleOp`](notes/annotations.md#cmd-teleop) | Registers the OpMode as a driver-controlled program so it shows up on the Driver Station | 🏷️ Annotations |
| [`{ }`](notes/program-structure.md#cmd-sym-123-125) | Braces: mark where a class or method starts and ends; they always come in pairs | 🏗️ Program Structure |

## 🛠️ How to update

The data lives in [`data/`](data): [`categories.csv`](data/categories.csv), [`commands.csv`](data/commands.csv) and [`parameters.csv`](data/parameters.csv). After editing them, run:

```bash
python3 scripts/build.py
```

This rebuilds this README, the notes in [`notes/`](notes) and the web page in [`docs/`](docs).

> 💡 To publish the web page: **Settings → Pages → Branch `main` / folder `/docs`**.
