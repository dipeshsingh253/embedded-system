# Voltage

## What Is Voltage?

**Voltage** is electrical pressure or "push." It's the force that makes electrons want to flow from one place to another.

Just as water pressure pushes water through pipes, voltage pushes electrons through wires.

> **Voltage = Electrical Pressure**

## Voltage Is Always a Difference

Here's something crucial to understand: **Voltage is always measured between two points.**

You can't talk about the voltage "at" a single point—you must specify two points and measure the difference between them.

### Examples

❌ **Wrong:** "The voltage at point A is 5V"
✅ **Correct:** "The voltage between point A and point B is 5V"
✅ **Correct:** "Point A is 5V higher than point B"

Think of it like height:
- You can't say a mountain is "1000m tall" without specifying: tall compared to what?
- Sea level? Base of the mountain? Center of Earth?
- Similarly, voltage needs a reference point

### Ground as Reference

In electronics, we often use **ground** (marked as ⏚ or GND) as the reference point (like sea level for height):

```
         +5V ← "5 volts above ground"
         │
        ─┴─  ← Ground (0V reference)
```

When we say "5V," we usually mean "5 volts higher than ground."

## The Unit: Volts (V)

Voltage is measured in **Volts**, abbreviated as **V**.

Named after Alessandro Volta, who invented the first battery.

### Common Voltage Examples

| Source | Voltage |
|--------|---------|
| AA battery | 1.5V |
| AAA battery | 1.5V |
| 9V battery | 9V |
| USB port | 5V |
| Phone charger | 5V |
| Laptop charger | 19V (typical) |
| Car battery | 12V |
| US wall outlet | 120V AC |
| Europe wall outlet | 230V AC |
| Static shock | 1,000 - 10,000V |
| Lightning | 100,000,000V |

⚠️ **Safety note**: High voltage can be dangerous! Wall outlets (120V) can kill. Always be careful with mains electricity.

## How Batteries Create Voltage

Remember from [04-battery-working.md](./04-battery-working.md):

- Battery uses chemical reactions to separate charges
- **Anode (-)**: Excess electrons pile up
- **Cathode (+)**: Shortage of electrons
- This separation creates an electric field
- The field strength = voltage

```
    Anode          Cathode
      ⊖              ⊕
     (-)            (+)
   More e⁻   ←──→   Fewer e⁻
   
   Lower           Higher
   pressure        pressure
   
   ← Voltage = Pressure difference →
```

The voltage tells you how much "pressure" is pushing electrons from negative to positive.

## Water Tank Height Analogy

Voltage is perfectly analogous to water pressure from height:

### Tall Tank (High Voltage)
```
    ╔═══════╗
    ║  10m  ║
    ║       ║  High pressure
    ║ Water ║  (like 9V)
    ╚═══╤═══╝
        │
        ↓ Strong flow
```

### Short Tank (Low Voltage)
```
    ╔═══════╗
    ║  2m   ║  Low pressure
    ║ Water ║  (like 1.5V)
    ╚═══╤═══╝
        │
        ↓ Weak flow
```

### The Analogy

| Water System | Electrical System |
|-------------|-------------------|
| Height difference | Voltage |
| Water flow rate | Current |
| Pipe resistance | Resistance |
| Gravity pulls water down | Voltage pushes electrons |
| Higher tank → stronger flow | Higher voltage → more current |

## Voltage Creates Current

Voltage is the **cause**, current is the **effect**:

```
Voltage (pressure) → Current (flow)
```

- **No voltage** → No pressure → No flow
- **Small voltage** → Small pressure → Small flow
- **Large voltage** → Large pressure → Large flow

But there's more to the story—resistance also matters (we'll learn that in [07-resistance.md](./07-resistance.md)).

## Voltage in a Circuit

Here's a simple circuit:

```
        ⊖  9V  ⊕
        -     +
        │     │
        │    💡 ← Light bulb
        │     │
        └─────┘
```

What's happening:
1. Battery creates 9V of pressure
2. Negative terminal has high "electron pressure"
3. Positive terminal has low "electron pressure"
4. Electrons flow from high to low pressure
5. Flow goes through the light bulb
6. Bulb lights up!

The voltage (9V) is what **drives** the current through the bulb.

## Voltage Doesn't Get "Used Up"

This is a common misconception: **Voltage doesn't get used up as it goes through a circuit.**

Think about water again:
- Height difference makes water flow
- Water falls from high to low
- The water itself moves, but the height difference remains

Similarly:
- Voltage difference makes electrons flow
- Electrons move from negative to positive
- The voltage difference remains (until battery dies)

### What Does Get "Used"?

**Energy** gets used. As electrons flow through components:
- Energy converts to light (LED)
- Energy converts to heat (resistor)
- Energy converts to motion (motor)

But the voltage (pressure) across the battery stays constant.

## Series vs Parallel Batteries

### Series: Voltages Add
```
  1.5V     1.5V     1.5V
   ⊖⊕       ⊖⊕       ⊖⊕
   ─┴─  ─  ─┴─  ─  ─┴─
   
   Total: 1.5V + 1.5V + 1.5V = 4.5V
```

Connecting batteries end-to-end (- to +) adds their voltages.

### Parallel: Voltage Stays Same
```
   ⊖⊕  1.5V
   ─┬─
    ├──── Both at 1.5V
   ─┴─
   ⊖⊕  1.5V
   
   Total: 1.5V (but more capacity)
```

Connecting batteries side-by-side keeps the same voltage but provides more current capacity.

## Measuring Voltage

To measure voltage, we use a **voltmeter** (or multimeter in voltage mode):

- Connect the **red probe** to the higher voltage point
- Connect the **black probe** to the lower voltage point (often ground)
- The meter shows the voltage difference

```
       +9V
        │
        ├──── Red probe
        │
    Voltmeter
        │
        ├──── Black probe
        │
       GND (0V)
       
    Display: 9.0V
```

## Key Takeaways

✅ **Voltage is electrical pressure** that pushes electrons

✅ Voltage is **always measured between two points** (a difference)

✅ Unit: **Volts (V)**

✅ Common examples: AA battery (1.5V), USB (5V), wall outlet (120V)

✅ Batteries create voltage through **charge separation**

✅ Like **water tank height** - higher = more pressure

✅ Voltage is the **cause**, current is the **effect**

✅ Voltage doesn't get "used up"—**energy** gets used

✅ Series batteries: voltages **add**

✅ Parallel batteries: voltage **stays same**

## What's Next?

You now understand voltage—the electrical pressure. But what about the flow itself? How do we measure how many electrons are flowing?

➡️ Continue to [06-current.md](./06-current.md)
