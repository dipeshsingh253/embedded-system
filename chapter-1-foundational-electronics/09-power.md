# Power

## What Is Power?

**Power** is the rate at which energy is used or converted. In electrical circuits, power tells you how much electrical energy is being converted to other forms (heat, light, motion, sound) every second.

> **Power = Energy Used Per Second**

## The Unit: Watts (W)

Power is measured in **Watts**, abbreviated as **W**.

Named after James Watt, the inventor who improved the steam engine.

### What Is One Watt?

One watt means **one joule of energy used per second**.

```
1 Watt = 1 Joule / 1 Second
1 W = 1 J/s
```

### Common Power Examples

| Device | Power |
|--------|-------|
| Small LED | 0.1 W (100 mW) |
| Phone charging | 5-10 W |
| LED light bulb | 10 W |
| Laptop | 50-100 W |
| Incandescent bulb | 60 W |
| Gaming desktop | 500-800 W |
| Microwave | 1000 W (1 kW) |
| Hair dryer | 1500 W (1.5 kW) |
| Electric car charging | 7000 W (7 kW) |

## The Power Formula: P = V × I

The fundamental formula for electrical power:

```
P = V × I
```

Where:
- **P** = Power (Watts)
- **V** = Voltage (Volts)
- **I** = Current (Amperes)

**Power equals voltage times current**

## Why P = V × I?

Let's understand why this formula makes sense:

### Breaking It Down

Remember:
- **Voltage (V)** = Energy per unit charge (Joules per Coulomb)
- **Current (I)** = Charge per unit time (Coulombs per second)

Multiply them:
```
V × I = (Joules/Coulomb) × (Coulombs/second)
      = Joules/second
      = Watts (Power!)
```

### Intuitive Understanding

```
Energy per charge × Charge per second = Energy per second

More voltage → More energy per electron
More current → More electrons per second
Together → More total energy used
```

Think of it like water:
- **Pressure × Flow = Power**
- High pressure water at high flow → Lots of power
- Can do more work (turn turbines, cut metal, etc.)

## Alternative Power Formulas

Using Ohm's Law (V = I × R), we can derive other useful forms:

### Formula 2: P = I²R

If you know current and resistance:

```
P = I²R = I × I × R
```

**Derivation:**
```
P = V × I
V = I × R  (Ohm's Law)
Therefore: P = (I × R) × I = I²R
```

### Formula 3: P = V²/R

If you know voltage and resistance:

```
P = V²/R = (V × V) / R
```

**Derivation:**
```
P = V × I
I = V / R  (Ohm's Law)
Therefore: P = V × (V / R) = V²/R
```

### Which Formula to Use?

Choose based on what you know:

| You Know | Use Formula |
|----------|-------------|
| Voltage and Current | P = V × I |
| Current and Resistance | P = I²R |
| Voltage and Resistance | P = V²/R |

All three give the same answer—use the most convenient!

## Where Does the Power Go?

Electrical power is converted to other forms of energy:

### 1. Heat 🔥
- Resistors convert electrical energy to heat
- This is usually **unwanted** (wasted energy)
- Why components get hot

### 2. Light 💡
- LEDs, light bulbs
- Some heat (less efficient)
- Some light (desired)

### 3. Motion ⚙️
- Motors convert electrical to mechanical
- Fans, drills, car wheels

### 4. Sound 🔊
- Speakers convert electrical to sound
- Also some heat (wasted)

### 5. Chemical Energy 🔋
- Charging batteries
- Electrical → Chemical (stored)

### 6. Other Forms
- Radio waves (WiFi, radio)
- Computation (CPU, logic)
- Displays (screens)

## Why Things Get Hot: I²R Heating

Notice that power dissipated as heat in a resistor is:

```
P = I²R
```

This is called **Joule heating** or **I²R heating**.

### Key Insight: Current Squared!

Power increases with the **square** of the current:

```
If I doubles → Power increases by 4×
If I triples → Power increases by 9×
If I 10× → Power increases by 100×!
```

**Example:**
```
1A through 10Ω: P = (1)² × 10 = 10W
2A through 10Ω: P = (2)² × 10 = 40W  ← 4× more heat!
3A through 10Ω: P = (3)² × 10 = 90W  ← 9× more heat!
```

This is why:
- High current causes more heating
- Wires melt with too much current
- Power lines use high voltage (low current) to reduce losses

## Example Calculations

### Example 1: LED Power

An LED operates at 3V and draws 20mA. What's the power consumption?

```
Given:
- V = 3V
- I = 20mA = 0.02A
- P = ?

Solution:
P = V × I
P = 3V × 0.02A
P = 0.06W = 60mW

Answer: 60 milliwatts
```

### Example 2: Resistor Heating

A 100Ω resistor has 9V across it. How much power does it dissipate as heat?

```
Given:
- R = 100Ω
- V = 9V
- P = ?

Solution (using P = V²/R):
P = V²/R
P = (9V)² / 100Ω
P = 81 / 100
P = 0.81W

Answer: 0.81 watts of heat
```

### Example 3: Phone Charger

A USB charger provides 5V and the phone draws 2A. What's the charging power?

```
Given:
- V = 5V
- I = 2A
- P = ?

Solution:
P = V × I
P = 5V × 2A
P = 10W

Answer: 10 watts
```

### Example 4: From Current and Resistance

5A flows through a 20Ω resistor. What's the power dissipated?

```
Given:
- I = 5A
- R = 20Ω
- P = ?

Solution (using P = I²R):
P = I²R
P = (5A)² × 20Ω
P = 25 × 20
P = 500W

Answer: 500 watts (gets very hot!)
```

### Example 5: Light Bulb

A 60W light bulb is plugged into a 120V outlet. How much current does it draw?

```
Given:
- P = 60W
- V = 120V
- I = ?

Solution (rearrange P = V × I):
I = P / V
I = 60W / 120V
I = 0.5A

Answer: 0.5 amperes (500mA)
```

## Power Ratings

Components have **power ratings**—the maximum power they can handle:

### Resistors

| Power Rating | Size | Use |
|--------------|------|-----|
| 1/8 W (0.125W) | Tiny | Low power circuits |
| 1/4 W (0.25W) | Small | Standard circuits |
| 1/2 W (0.5W) | Medium | Higher power |
| 1 W | Large | Significant power |
| 5 W | Very large | High power applications |

**Important**: Always use a resistor rated for **more** than the actual power!

**Safety margin**: Use at least 2× the calculated power:
- Calculate: 0.5W dissipated
- Use: 1W (or higher) resistor

### Example: Choosing a Resistor

You calculate a resistor will dissipate 0.3W. What rating should you use?

```
Calculated: 0.3W
Safety margin: 2× = 0.6W
Choose: 1W resistor (next standard size above 0.6W)
```

## Electrical Cost: Kilowatt-Hours

Your electric bill is based on energy used, measured in **kilowatt-hours** (kWh):

```
Energy (kWh) = Power (kW) × Time (hours)
```

### Example: Monthly Cost

A laptop uses 60W and runs 8 hours per day. How much energy per month at $0.12/kWh?

```
Power: 60W = 0.06kW
Hours per month: 8 hrs/day × 30 days = 240 hours

Energy = 0.06kW × 240hr = 14.4 kWh
Cost = 14.4 kWh × $0.12/kWh = $1.73/month
```

## Power Efficiency

**Efficiency** is the ratio of useful power out to total power in:

```
Efficiency = (Useful Power Out / Total Power In) × 100%
```

### Example: LED vs Incandescent

**LED bulb:**
- Input: 10W
- Light output: 8W
- Heat waste: 2W
- Efficiency: 8W/10W = 80%

**Incandescent bulb:**
- Input: 60W
- Light output: 3W
- Heat waste: 57W
- Efficiency: 3W/60W = 5%

LEDs are much more efficient!

## Real-World Applications

### 1. Sizing Power Supplies
Calculate total power needed for all components

### 2. Heat Management
High power → Need cooling (heatsinks, fans)

### 3. Battery Life
Lower power → Longer battery life

### 4. Component Selection
Choose components with adequate power ratings

### 5. Energy Efficiency
Reduce power to save money and environment

### 6. Circuit Protection
Fuses and breakers rated for power/current

## Key Takeaways

✅ **Power = Energy used per second** (rate of energy conversion)

✅ Unit: **Watts (W)**

✅ Basic formula: **P = V × I**

✅ Alternative formulas: **P = I²R** and **P = V²/R**

✅ Power converts to: **heat, light, motion, sound**, etc.

✅ **I²R heating**: Power increases with square of current

✅ Components have **power ratings** - don't exceed them!

✅ Use **safety margin** (2× calculated power minimum)

✅ High current causes **more heating** than high voltage

✅ **Efficiency** = useful power / total power

✅ Electricity cost based on **kWh** (power × time)

## What's Next?

You now understand the fundamental concepts and formulas! But working with electronics means dealing with many different unit scales. Let's learn about metric prefixes and unit conversions.

➡️ Continue to [10-units-and-conversions.md](./10-units-and-conversions.md)
