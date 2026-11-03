# 🎮 Gamepad

> Read the driver's controllers: buttons, joysticks and triggers through gamepad1 and gamepad2.

**5** items · **10** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Item | What it does |
|:--|:--|
| [`gamepad1 / gamepad2`](#cmd-gamepad1-gamepad2) | The two controllers the Driver Station recognizes; each one is a Gamepad object |
| [`Dot access (.)`](#cmd-dot-access) | controller.part: the dot reads one part of the controller; read it as "of" |
| [`Buttons (a, b, x, y)`](#cmd-buttons-a-b-x-y) | Return a boolean: true while pressed, false when released |
| [`Joysticks`](#cmd-joysticks) | Return a decimal from -1.0 to 1.0; 0.0 is the center |
| [`Triggers`](#cmd-triggers) | Decimal from 0.0 (released) to 1.0 (pressed all the way); never negative |

---

<a id="cmd-gamepad1-gamepad2"></a>

## `gamepad1 / gamepad2`

The two controllers the Driver Station recognizes; each one is a Gamepad object

```java
boolean disparar = gamepad2.a;
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `Start + A` | Pressed together, they register the controller as gamepad1 | `boolean a1 = gamepad1.a;` |
| `Start + B` | Pressed together, they register the controller as gamepad2 | `boolean a2 = gamepad2.a;` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-dot-access"></a>

## `Dot access (.)`

controller.part: the dot reads one part of the controller; read it as "of"

```java
double gatillo = gamepad1.right_trigger;
```

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-buttons-a-b-x-y"></a>

## `Buttons (a, b, x, y)`

Return a boolean: true while pressed, false when released

```java
boolean botonA = gamepad1.a;
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `dpad_up / dpad_down / dpad_left / dpad_right` | The D-pad works as four boolean buttons | `boolean arriba = gamepad1.dpad_up;` |
| `left_bumper / right_bumper` | Top buttons; also boolean | `boolean bumper = gamepad1.right_bumper;` |
| `start / back` | Center buttons; also boolean | `boolean inicio = gamepad1.start;` |
| `left_stick_button / right_stick_button` | true when you press the stick down | `boolean click = gamepad1.left_stick_button;` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-joysticks"></a>

## `Joysticks`

Return a decimal from -1.0 to 1.0; 0.0 is the center

```java
double avance = gamepad1.left_stick_y;
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `_x (horizontal axis)` | Left is -1.0 and right is 1.0 | `double giro = gamepad1.left_stick_x;` |
| `_y (vertical axis)` | Up is -1.0 and down is 1.0 (the opposite of what you'd expect) | `double avance = -gamepad1.left_stick_y;` |
| `left_ / right_` | Picks the left or the right stick | `double giro = gamepad1.right_stick_x;` |
| `(float type)` | In the FTC SDK they are float; they fit in a double with no problem | `double y = gamepad1.left_stick_y;` |

<sub>[⬆ Back to top](#commands)</sub>

---

<a id="cmd-triggers"></a>

## `Triggers`

Decimal from 0.0 (released) to 1.0 (pressed all the way); never negative

```java
double succion = gamepad1.right_trigger;
```

<sub>[⬆ Back to top](#commands)</sub>
