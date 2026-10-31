<div align="center">

# ☕ Java Scripting

**A personal reference for learning Java (with FTC robotics in mind): keywords, syntax and concepts, with examples that compile.**

![Concepts](https://img.shields.io/badge/concepts-25-2ea44f?style=for-the-badge) ![Parameters](https://img.shields.io/badge/parameters-13-0969da?style=for-the-badge) ![Categories](https://img.shields.io/badge/categories-6-8250df?style=for-the-badge)

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
| 🔤 | **[Strings & Types](notes/strings-types.md)** | Working with text and data types. | `.equals()` |

## 🔤 A–Z index

| Item | What it does | Category |
|:--|:--|:--|
| [`Case sensitivity`](notes/program-structure.md#cmd-case-sensitivity) | Java tells upper and lower case apart: potencia and Potencia are different names; keywords are always lowercase | 🏗️ Program Structure |
| [`class`](notes/program-structure.md#cmd-class) | Defines a class: the container where all Java code lives | 🏗️ Program Structure |
| [`extends`](notes/program-structure.md#cmd-extends) | Inheritance: the child class gets everything the parent class already has | 🏗️ Program Structure |
| [`File name = class name`](notes/program-structure.md#cmd-file-name-class-name) | A public class must have the same name as its .java file, capital letters included | 🏗️ Program Structure |
| [`import`](notes/program-structure.md#cmd-import) | Brings in a class from a library (like the FTC SDK) so you can use it in the file | 🏗️ Program Structure |
| [`init()`](notes/methods.md#cmd-init) | Runs once when INIT is pressed; used to get the robot ready | ⚙️ Methods |
| [`loop()`](notes/methods.md#cmd-loop) | Repeats about 50 times per second while the OpMode is running | ⚙️ Methods |
| [`PascalCase`](notes/program-structure.md#cmd-pascalcase) | Naming convention for classes: every word starts with a capital letter | 🏗️ Program Structure |
| [`public`](notes/program-structure.md#cmd-public) | Access modifier: lets other classes and the robot's system use the class or method | 🏗️ Program Structure |
| [`return`](notes/methods.md#cmd-return) | Sends a value back from a method that isn't void and ends it | ⚙️ Methods |
| [`telemetry.addData()`](notes/telemetry.md#cmd-telemetry-adddata) | Sends a label and a value to the Driver Station screen for debugging | 📡 Telemetry |
| [`void`](notes/methods.md#cmd-void) | Return type: the method does its job but gives no value back | ⚙️ Methods |
| [`Whitespace`](notes/program-structure.md#cmd-whitespace) | Java ignores spaces, tabs and line breaks; blocks are marked by braces, not indentation | 🏗️ Program Structure |
| [`( )`](notes/program-structure.md#cmd-sym-40-41) | Every opening parenthesis needs a closing one; if one is missing, the program won't compile | 🏗️ Program Structure |
| [`.equals()`](notes/strings-types.md#cmd-equals) | Compares the text of two Strings; == only checks whether they are the same object | 🔤 Strings & Types |
| [`/* */`](notes/comments.md#cmd-sym-47-42-42-47) | Block comment: ignores everything between /* and */, even across several lines | 💬 Comments |
| [`/** */`](notes/comments.md#cmd-sym-47-42-42-42-47) | Javadoc: a block comment that tools read to generate documentation and hover tooltips | 💬 Comments |
| [`//`](notes/comments.md#cmd-sym-47-47) | Single-line comment: the compiler ignores everything after it on that line | 💬 Comments |
| [`;`](notes/program-structure.md#cmd-sym-59) | Ends every statement; lines that open a brace { don't take one | 🏗️ Program Structure |
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
