# Ohm's Law

## The Most Important Formula in Electronics

**Ohm's Law** describes the relationship between voltage, current, and resistance. It's the foundation of circuit analysis and the first formula every electronics enthusiast must master.

> **V = I × R**

Where:
- **V** = Voltage (Volts)
- **I** = Current (Amperes)
- **R** = Resistance (Ohms)

## The Three Forms

Ohm's Law can be rearranged to solve for any of the three variables:

### 1. Voltage (V)
```
V = I × R
```
Voltage equals current times resistance

**Example**: If 2A flows through 5Ω:
```
V = 2A × 5Ω = 10V
```

### 2. Current (I)
```
I = V / R
```
Current equals voltage divided by resistance

**Example**: If 10V is across 5Ω:
```
I = 10V / 5Ω = 2A
```

### 3. Resistance (R)
```
R = V / I
```
Resistance equals voltage divided by current

**Example**: If 10V pushes 2A:
```
R = 10V / 2A = 5Ω
```

## The Memory Triangle

A helpful visual to remember Ohm's Law:

```
      V
    ─────
    │   │
    │   │
    ─────
    I   R
```

**How to use it:**
- Cover the variable you want to find
- What remains shows the formula

**Examples:**

Cover **V**: See I × R → **V = I × R**
```
      ▓
    ─────
    │   │
    │   │
    ─────
    I   R
```

Cover **I**: See V / R → **I = V / R**
```
      V
    ─────
    │   │
    │ ▓ │
    ─────
        R
```

Cover **R**: See V / I → **R = V / I**
```
      V
    ─────
    │   │
    │   │
    ─────
    I   ▓
```

## Intuitive Understanding

### More Voltage → More Current
If you increase voltage (pressure) while keeping resistance constant:
```
5V / 10Ω = 0.5A
10V / 10Ω = 1.0A  ← Double voltage → Double current
20V / 10Ω = 2.0A  ← 4× voltage → 4× current
```

Like water: more pressure → more flow

### More Resistance → Less Current
If you increase resistance while keeping voltage constant:
```
10V / 5Ω = 2.0A
10V / 10Ω = 1.0A  ← Double resistance → Half current
10V / 20Ω = 0.5A  ← 4× resistance → 1/4 current
```

Like water: narrower pipe → less flow

### Both Together
```
V = I × R

More voltage → More current
More resistance → Less current
```

Think: "Voltage pushes, resistance opposes"

## Water Flow Analogy

Ohm's Law perfectly matches water hydraulics:

```
Pressure = Flow Rate × Pipe Resistance
   V     =     I     ×       R

High pressure → High flow (if pipe is open)
Narrow pipe → Low flow (even with high pressure)
```

| Water | Electricity |
|-------|------------|
| Water pressure | Voltage (V) |
| Flow rate (liters/sec) | Current (I) |
| Pipe resistance/friction | Resistance (R) |
| Pressure = Flow × Resistance | V = I × R |

## Practical Examples

### Example 1: LED Circuit

You want to light an LED with a 9V battery. The LED needs 20mA (0.02A) to light properly. What resistor do you need?

```
Circuit:
  ⊖ 9V ⊕
  │    │
  R    💡 LED (needs 20mA)
  │    │
  └────┘

Given:
- V = 9V (battery voltage)
- I = 0.02A (20mA, desired current)
- R = ?

Solve for R:
R = V / I
R = 9V / 0.02A
R = 450Ω

Answer: Use a 450Ω resistor
```

### Example 2: Short Circuit Danger

What happens if you connect a 9V battery directly to a wire with almost no resistance (0.01Ω)?

```
Given:
- V = 9V
- R = 0.01Ω (essentially a short circuit)
- I = ?

Solve for I:
I = V / R
I = 9V / 0.01Ω
I = 900A

Danger! 900 Amperes!
```

This massive current would:
- Heat the wire instantly
- Melt the wire
- Drain the battery immediately
- Possibly cause fire or explosion

**This is why short circuits are dangerous!** Always have appropriate resistance in your circuit.

### Example 3: Voltage Drop Across Resistor

You have a 100Ω resistor and 50mA (0.05A) flowing through it. What's the voltage drop across the resistor?

```
Given:
- R = 100Ω
- I = 0.05A (50mA)
- V = ?

Solve for V:
V = I × R
V = 0.05A × 100Ω
V = 5V

Answer: 5V drop across the resistor
```

### Example 4: Checking Circuit Current

You measure 12V across a 1kΩ (1000Ω) resistor. How much current is flowing?

```
Given:
- V = 12V
- R = 1000Ω
- I = ?

Solve for I:
I = V / R
I = 12V / 1000Ω
I = 0.012A = 12mA

Answer: 12 milliamperes
```

### Example 5: Calculating Required Resistance

You have a 5V USB port and want 100mA (0.1A) to flow. What resistance do you need?

```
Given:
- V = 5V
- I = 0.1A
- R = ?

Solve for R:
R = V / I
R = 5V / 0.1A
R = 50Ω

Answer: 50Ω resistor
```

## Common Mistakes to Avoid

### Mistake 1: Unit Confusion
❌ **Wrong**: V = 20mA × 1kΩ = 20
✅ **Correct**: Convert first!
```
20mA = 0.02A
1kΩ = 1000Ω
V = 0.02A × 1000Ω = 20V
```

Always convert to base units (A, V, Ω) before calculating!

### Mistake 2: Dividing the Wrong Way
❌ **Wrong**: I = R / V
✅ **Correct**: I = V / R

Use the triangle to avoid this mistake!

### Mistake 3: Ignoring LED Voltage Drop
When calculating LED resistors, remember LEDs have their own voltage drop (~2V). The resistor only sees the remaining voltage!

```
9V battery with LED:
- LED drops ~2V
- Resistor sees: 9V - 2V = 7V
- Use 7V in Ohm's Law, not 9V!
```

## Practice Problems

Try these yourself before looking at answers!

### Problem 1
A 12V car battery pushes current through a 4Ω resistance. How much current flows?

### Problem 2
A component needs 500mA at 5V. What's its resistance?

### Problem 3
3A flows through a 15Ω resistor. What's the voltage across it?

### Problem 4
A circuit has 9V and needs exactly 30mA. What resistor value is required?

---

### Answers

**Problem 1:**
```
I = V / R = 12V / 4Ω = 3A
```

**Problem 2:**
```
R = V / I = 5V / 0.5A = 10Ω
```

**Problem 3:**
```
V = I × R = 3A × 15Ω = 45V
```

**Problem 4:**
```
R = V / I = 9V / 0.03A = 300Ω
```

## When Ohm's Law Doesn't Apply

Ohm's Law works for **linear resistive components** (resistors, wires). It doesn't directly apply to:

- **LEDs** - Have non-linear voltage-current relationship
- **Batteries** - Source voltage, not resistive
- **Capacitors** - Time-dependent behavior
- **Inductors** - Time-dependent behavior
- **Diodes** - Non-linear
- **Transistors** - Complex behavior

For these components, we use other formulas and models. But Ohm's Law still applies to the resistive parts of circuits containing these components.

## Real-World Applications

### 1. Designing LED Circuits
Calculate resistor needed for proper LED brightness

### 2. Circuit Troubleshooting
Measure voltage and resistance to find current

### 3. Power Supply Design
Determine current capability needed

### 4. Fuse Selection
Calculate expected current to choose proper fuse rating

### 5. Wire Sizing
Calculate voltage drop to select appropriate wire thickness

## Key Takeaways

✅ **V = I × R** is the fundamental relationship

✅ Can be rearranged: **I = V / R** and **R = V / I**

✅ More voltage → More current (if R is constant)

✅ More resistance → Less current (if V is constant)

✅ Use the **triangle memory aid** to remember formulas

✅ Always convert to **base units** before calculating

✅ **Short circuits** (low R) cause dangerous high currents

✅ Applies to **resistive components** (not LEDs, batteries, etc.)

✅ Essential for **circuit design** and **troubleshooting**

## What's Next?

Now you can calculate voltage, current, and resistance! But there's another important quantity in electronics: **power**. How much energy is being used? Why do things get hot?

➡️ Continue to [09-power.md](./09-power.md)
