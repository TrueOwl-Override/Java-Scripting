# 📡 Telemetry

> Send data from the robot to the Driver Station screen to see what it's doing.

**1** items · **2** parameters  ·  [⬅ Back to index](../README.md)

<a id="commands"></a>

| Item | What it does |
|:--|:--|
| [`telemetry.addData()`](#cmd-telemetry-adddata) | Sends a label and a value to the Driver Station screen for debugging |

---

<a id="cmd-telemetry-adddata"></a>

## `telemetry.addData()`

Sends a label and a value to the Driver Station screen for debugging

```java
telemetry.addData("Hello", "World");
```

| Parameter | What it does | Example |
|:--|:--|:--|
| `caption` | First argument: the label shown on the left of the screen | `telemetry.addData("Distancia", 25);` |
| `value` | Second argument: the data to show (text, number or variable) | `telemetry.addData("Velocidad", 0.5);` |

<sub>[⬆ Back to top](#commands)</sub>
