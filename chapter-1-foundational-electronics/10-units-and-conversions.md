# Units and Conversions

## Basic Units in Electronics

### The Core Four

| Quantity | Symbol | Unit | Unit Symbol |
|----------|--------|------|-------------|
| **Voltage** | V | Volt | V |
| **Current** | I | Ampere (Amp) | A |
| **Resistance** | R | Ohm | Ω |
| **Power** | P | Watt | W |

### Other Important Units

| Quantity | Symbol | Unit | Unit Symbol |
|----------|--------|------|-------------|
| **Charge** | Q | Coulomb | C |
| **Time** | t | Second | s |
| **Capacitance** | C | Farad | F |
| **Inductance** | L | Henry | H |
| **Frequency** | f | Hertz | Hz |
| **Energy** | E | Joule | J |

## Metric Prefixes

Electronics uses the metric system with standard prefixes. You **must** memorize these!

### The Complete Table

| Prefix | Symbol | Multiplier | Power of 10 | Decimal |
|--------|--------|------------|-------------|---------|
| **Tera** | T | 1,000,000,000,000 | 10¹² | 1 trillion |
| **Giga** | G | 1,000,000,000 | 10⁹ | 1 billion |
| **Mega** | M | 1,000,000 | 10⁶ | 1 million |
| **Kilo** | k | 1,000 | 10³ | 1 thousand |
| **(Base)** | - | 1 | 10⁰ | 1 |
| **Milli** | m | 0.001 | 10⁻³ | 1 thousandth |
| **Micro** | μ | 0.000001 | 10⁻⁶ | 1 millionth |
| **Nano** | n | 0.000000001 | 10⁻⁹ | 1 billionth |
| **Pico** | p | 0.000000000001 | 10⁻¹² | 1 trillionth |

### Memory Aids

**Large (going up by 1000×):**
```
Base → Kilo → Mega → Giga → Tera
  ×1000   ×1000   ×1000   ×1000
```

**Small (going down by 1000×):**
```
Base → Milli → Micro → Nano → Pico
  ÷1000    ÷1000    ÷1000   ÷1000
```

### Common Prefixes in Electronics

Most commonly used:

**Large values:**
- **k** (kilo) - thousands
- **M** (Mega) - millions

**Small values:**
- **m** (milli) - thousandths
- **μ** (micro) - millionths
- **n** (nano) - billionths
- **p** (pico) - trillionths

## Current Conversions

### Current Scale

```
        Tera (TA)
           ↓ ×1000
        Giga (GA)
           ↓ ×1000
        Mega (MA)
           ↓ ×1000
        Kilo (kA)
           ↓ ×1000
    >>> Ampere (A) <<<  ← Base unit
           ↓ ×1000
       Milli (mA)  ← Very common!
           ↓ ×1000
       Micro (μA)  ← Common
           ↓ ×1000
       Nano (nA)
           ↓ ×1000
       Pico (pA)
```

### Common Current Conversions

```
1 A = 1,000 mA
1 A = 1,000,000 μA
1 mA = 1,000 μA
1 mA = 0.001 A
1 μA = 0.001 mA
1 μA = 0.000001 A
```

### Current Examples

| Value | Conversion |
|-------|------------|
| 2 A | = 2,000 mA |
| 500 mA | = 0.5 A |
| 20 mA | = 0.02 A = 20,000 μA |
| 100 μA | = 0.1 mA = 0.0001 A |
| 0.05 A | = 50 mA |

## Voltage Conversions

### Voltage Scale

```
        Mega (MV)
           ↓ ×1000
        Kilo (kV)  ← High voltage power lines
           ↓ ×1000
    >>> Volt (V) <<<  ← Base unit, most common!
           ↓ ×1000
       Milli (mV)  ← Signal levels
           ↓ ×1000
       Micro (μV)  ← Small signals
```

### Common Voltage Conversions

```
1 V = 1,000 mV
1 V = 1,000,000 μV
1 kV = 1,000 V
1 mV = 0.001 V
1 mV = 1,000 μV
1 μV = 0.000001 V
```

### Voltage Examples

| Value | Conversion |
|-------|------------|
| 5 V | = 5,000 mV |
| 1.5 V | = 1,500 mV |
| 120 V | = 0.12 kV |
| 3300 mV | = 3.3 V |
| 50 mV | = 0.05 V = 50,000 μV |

## Resistance Conversions

### Resistance Scale

```
        Mega (MΩ)  ← Very high resistance
           ↓ ×1000
        Kilo (kΩ)  ← Very common!
           ↓ ×1000
    >>> Ohm (Ω) <<<  ← Base unit
           ↓ ×1000
       Milli (mΩ)  ← Very low resistance
```

### Common Resistance Conversions

```
1 MΩ = 1,000 kΩ
1 MΩ = 1,000,000 Ω
1 kΩ = 1,000 Ω
1 kΩ = 0.001 MΩ
1 Ω = 1,000 mΩ
1 Ω = 0.001 kΩ
```

### Resistance Examples

| Value | Conversion |
|-------|------------|
| 1 kΩ | = 1,000 Ω |
| 4.7 kΩ | = 4,700 Ω |
| 1 MΩ | = 1,000 kΩ = 1,000,000 Ω |
| 470 Ω | = 0.47 kΩ |
| 10,000 Ω | = 10 kΩ |

## Power Conversions

### Power Scale

```
        Mega (MW)  ← Power plants
           ↓ ×1000
        Kilo (kW)  ← House appliances
           ↓ ×1000
    >>> Watt (W) <<<  ← Base unit, common!
           ↓ ×1000
       Milli (mW)  ← Small electronics
           ↓ ×1000
       Micro (μW)  ← Very low power
```

### Common Power Conversions

```
1 kW = 1,000 W
1 W = 1,000 mW
1 W = 1,000,000 μW
1 mW = 0.001 W
1 mW = 1,000 μW
```

### Power Examples

| Value | Conversion |
|-------|------------|
| 1.5 kW | = 1,500 W |
| 60 W | = 60,000 mW = 0.06 kW |
| 500 mW | = 0.5 W |
| 100 mW | = 0.1 W |

## Quick Reference Tables

### Current

| Amperes (A) | Milliamperes (mA) | Microamperes (μA) |
|-------------|-------------------|-------------------|
| 1 A | 1,000 mA | 1,000,000 μA |
| 0.1 A | 100 mA | 100,000 μA |
| 0.01 A | 10 mA | 10,000 μA |
| 0.001 A | 1 mA | 1,000 μA |
| 0.0001 A | 0.1 mA | 100 μA |

### Resistance

| Ohms (Ω) | Kilohms (kΩ) | Megohms (MΩ) |
|----------|--------------|--------------|
| 1,000,000 Ω | 1,000 kΩ | 1 MΩ |
| 100,000 Ω | 100 kΩ | 0.1 MΩ |
| 10,000 Ω | 10 kΩ | 0.01 MΩ |
| 1,000 Ω | 1 kΩ | 0.001 MΩ |
| 100 Ω | 0.1 kΩ | 0.0001 MΩ |

### Power

| Watts (W) | Milliwatts (mW) | Kilowatts (kW) |
|-----------|-----------------|----------------|
| 1,000 W | 1,000,000 mW | 1 kW |
| 100 W | 100,000 mW | 0.1 kW |
| 10 W | 10,000 mW | 0.01 kW |
| 1 W | 1,000 mW | 0.001 kW |
| 0.1 W | 100 mW | 0.0001 kW |

## Conversion Method

### Method 1: Using the Ladder (Up or Down)

Each step is ×1000 (going up) or ÷1000 (going down):

**Example**: Convert 5000 mA to A

```
Start: 5000 mA
Go up one step to A: ÷1000
5000 ÷ 1000 = 5 A
```

**Example**: Convert 2.5 A to μA

```
Start: 2.5 A
Go down two steps (A → mA → μA): ×1000 twice
2.5 × 1000 = 2500 mA
2500 × 1000 = 2,500,000 μA
```

### Method 2: Direct Multiplication

**Going smaller** (A to mA to μA): **Multiply**
```
A → mA: ×1,000
A → μA: ×1,000,000
mA → μA: ×1,000
```

**Going larger** (μA to mA to A): **Divide**
```
mA → A: ÷1,000
μA → A: ÷1,000,000
μA → mA: ÷1,000
```

### Method 3: Move Decimal Point

Each factor of 1000 = move decimal 3 places

**Example**: 450 Ω to kΩ
```
450 Ω → kΩ (going up, divide by 1000)
Move decimal 3 places left: 450. → 0.450 kΩ
```

**Example**: 2.5 kΩ to Ω
```
2.5 kΩ → Ω (going down, multiply by 1000)
Move decimal 3 places right: 2.500 → 2500 Ω
```

## Practice Conversions

Try these yourself!

### Set 1: Current
1. 20 mA → A
2. 2.5 A → mA
3. 500 μA → mA
4. 0.05 A → mA

### Set 2: Resistance
1. 450 Ω → kΩ
2. 1.5 kΩ → Ω
3. 2.2 MΩ → kΩ
4. 100,000 Ω → MΩ

### Set 3: Voltage
1. 5000 mV → V
2. 3.3 V → mV
3. 120 V → kV
4. 50 mV → V

### Set 4: Power
1. 0.18 W → mW
2. 500 mW → W
3. 2.5 kW → W
4. 100 mW → μW

---

### Answers

**Set 1: Current**
1. 20 mA = 0.02 A
2. 2.5 A = 2,500 mA
3. 500 μA = 0.5 mA
4. 0.05 A = 50 mA

**Set 2: Resistance**
1. 450 Ω = 0.45 kΩ
2. 1.5 kΩ = 1,500 Ω
3. 2.2 MΩ = 2,200 kΩ
4. 100,000 Ω = 0.1 MΩ

**Set 3: Voltage**
1. 5000 mV = 5 V
2. 3.3 V = 3,300 mV
3. 120 V = 0.12 kV
4. 50 mV = 0.05 V

**Set 4: Power**
1. 0.18 W = 180 mW
2. 500 mW = 0.5 W
3. 2.5 kW = 2,500 W
4. 100 mW = 100,000 μW

## Tips for Success

✅ **Memorize the common prefixes**: k, m, μ, M

✅ **Remember the factor**: 1000 between each step

✅ **Check if the number makes sense**: 
   - Going smaller units → Bigger number
   - Going bigger units → Smaller number

✅ **Use scientific notation** for very large/small numbers:
   - 0.000005 A = 5 × 10⁻⁶ A = 5 μA

✅ **Practice, practice, practice!** Do conversions daily until they're automatic

## Common Mistakes to Avoid

❌ Confusing M (Mega) with m (milli)
- M = million (×10⁶)
- m = thousandth (×10⁻³)

❌ Forgetting to convert units before calculations
- Always convert to base units first!
- Then calculate
- Then convert result back if needed

❌ Moving decimal wrong direction
- Smaller units → Multiply (bigger number)
- Larger units → Divide (smaller number)

## Key Takeaways

✅ **Basic units**: V (Volts), A (Amps), Ω (Ohms), W (Watts)

✅ **Common prefixes**: k (×1000), m (÷1000), μ (÷1,000,000), M (×1,000,000)

✅ **Factor of 1000** between adjacent prefixes

✅ **Always convert to base units** before doing Ohm's Law calculations

✅ **Practice conversions** until they become second nature

✅ **Check your work**: Does the result make sense?

## What's Next?

Now you have all the fundamental knowledge and can work with different unit scales! Let's review everything and test your understanding with practice problems.

➡️ Continue to [11-summary-and-practice.md](./11-summary-and-practice.md)
