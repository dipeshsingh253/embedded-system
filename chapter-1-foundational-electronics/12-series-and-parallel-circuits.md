# Series and Parallel Circuits

## Introduction

When building circuits, components can be connected in two fundamental ways: **series** or **parallel**. Understanding these connection types is crucial because they behave completely differently in terms of current, voltage, and resistance.

> **Series**: Components connected end-to-end in a single path  
> **Parallel**: Components connected across common points, creating multiple paths

## Series Circuits

### Definition

**Series circuits** are circuits where components are connected end-to-end in a single path, so the same current flows through all components.

```
    ⊕ Battery ⊖
    │         │
    R₁        │  ← One continuous path
    │         │
    R₂        │
    │         │
    R₃        │
    │         │
    └─────────┘

Single path: Current has no choice but to flow through all components
```

Think of it like a train on a single track—every train car (electron) must follow the same path through each station (component).

### Key Characteristics

#### 1. Current: Same Everywhere
In a series circuit, the **same current** flows through every component:

```
I₁ = I₂ = I₃ = Iₜₒₜₐₗ
```

**Why?** There's only one path, so all electrons must flow through each component.

**Example:**
```
     5A    5A    5A
  ───│────│────│───
     R₁   R₂   R₃
     
  All resistors see the same 5A current
```

Just like water in a single pipe—the flow rate is the same at every point.

#### 2. Voltage: Divided Among Components
The total voltage is **divided** among the components:

```
Vₜₒₜₐₗ = V₁ + V₂ + V₃ + ...
```

**Why?** Each component uses up some of the available voltage.

**Example:**
```
12V battery with three resistors:
  V₁ = 3V (across R₁)
  V₂ = 5V (across R₂)
  V₃ = 4V (across R₃)
  
  Total: 3V + 5V + 4V = 12V ✓
```

Like a waterfall in steps—the total height (voltage) is divided among each step (component).

#### 3. Resistance: Total is Sum of All
Total resistance is the **sum** of individual resistances:

```
Rₜₒₜₐₗ = R₁ + R₂ + R₃ + ...
```

**Why?** Current must pass through each resistance, so they add up.

**Example:**
```
R₁ = 100Ω
R₂ = 200Ω
R₃ = 300Ω

Rₜₒₜₐₗ = 100Ω + 200Ω + 300Ω = 600Ω
```

Each resistor adds to the total opposition to current flow.

#### 4. If One Component Fails, Entire Circuit Breaks

⚠️ **Critical characteristic**: If any component opens (breaks), the entire circuit stops working.

```
Working:
  ──R₁──R₂──R₃──  ← Current flows

One breaks:
  ──R₁──✗──R₃──   ← No current anywhere!
```

Like old Christmas lights—if one bulb burns out, the whole string goes dark.

### Applications

Series circuits are used when you want:

#### 1. Voltage Dividers
Split voltage into smaller values for different parts of a circuit:
```
12V ──┐
      R₁ (1kΩ)
      │
      ├── 6V output
      │
      R₂ (1kΩ)
      │
    ──┴── GND
```

#### 2. String Lights (Old Style)
Each bulb is in series. All light up together or none do.

#### 3. Safety Switches
Put switch in series so it can disconnect entire circuit:
```
Battery ──Switch──Load──GND

Open switch → Entire circuit off
```

#### 4. Current Limiting
Add resistor in series to limit current through sensitive components like LEDs.

## Parallel Circuits

### Definition

**Parallel circuits** are circuits where components are connected across common points, creating multiple paths for current to flow.

```
        ⊕ Battery ⊖
        │         │
    ┌───┴───┬─────┤
    │       │     │
    R₁      R₂    R₃  ← Three separate paths
    │       │     │
    └───┬───┴─────┤
        │         │
```

Think of it like multiple lanes on a highway—cars (electrons) can choose different paths, and traffic (current) divides among them.

### Key Characteristics

#### 1. Voltage: Same Across All Components
In a parallel circuit, **all components see the same voltage**:

```
V₁ = V₂ = V₃ = Vₜₒₜₐₗ
```

**Why?** All components are connected to the same two points (+ and -).

**Example:**
```
        12V
    ┌───┴───┬───┬───┐
    R₁      R₂  R₃  LED
   12V     12V 12V 12V
    │       │   │   │
    └───┬───┴───┴───┘

All components see full 12V
```

Like water pressure in pipes connected to the same faucet—all get the same pressure.

#### 2. Current: Divided Among Branches
The total current is **divided** among the branches:

```
Iₜₒₜₐₗ = I₁ + I₂ + I₃ + ...
```

**Why?** Current splits at junction points, taking multiple paths.

**Example:**
```
           10A total
        ┌───┴───┬───┬───┐
        R₁      R₂  R₃
        3A      4A  3A
        │       │   │
        └───┬───┴───┴───┘
            
Total: 3A + 4A + 3A = 10A ✓
```

Like a river splitting into multiple streams—the total water flow divides.

#### 3. Resistance: Total is Less Than Smallest
Total resistance uses the **reciprocal formula**:

```
1/Rₜₒₜₐₗ = 1/R₁ + 1/R₂ + 1/R₃ + ...
```

**Why?** More paths mean less total opposition (easier for current to flow).

**Example:**
```
Three 300Ω resistors in parallel:

1/Rₜₒₜₐₗ = 1/300 + 1/300 + 1/300
1/Rₜₒₜₐₗ = 3/300 = 1/100
Rₜₒₜₐₗ = 100Ω

100Ω < 300Ω → Total is less than any individual!
```

**Special case** (two equal resistors):
```
Rₜₒₜₐₗ = R/2
```

**Special case** (two resistors):
```
Rₜₒₜₐₗ = (R₁ × R₂) / (R₁ + R₂)
```

Adding more paths in parallel **always reduces** total resistance.

#### 4. Other Components Continue Working If One Fails

✅ **Major advantage**: If one component fails (opens), others keep working.

```
Working:
  ┌──R₁──┐
──┤      ├──  ← All work
  ├──R₂──┤
  └──R₃──┘

One breaks:
  ┌──R₁──┐
──┤      ├──  ← R₂ and R₃ still work!
  ├──✗───┤
  └──R₃──┘
```

Like modern Christmas lights—if one bulb fails, the rest stay lit.

### Applications

Parallel circuits are used when you want:

#### 1. Home Electrical Wiring
All outlets and lights in your home are parallel:
```
120V ┌───Outlet 1
     ├───Outlet 2
     ├───Light 1
     └───Light 2

Each works independently
```

Each device gets full voltage and can be turned on/off independently.

#### 2. Car Headlights
Both headlights are parallel:
```
12V ┌───Left Headlight
    └───Right Headlight

If one burns out, the other still works
```

#### 3. Battery Banks
Batteries in parallel increase capacity (amp-hours):
```
    ┌───Battery 1 (12V, 100Ah)
12V ┤
    └───Battery 2 (12V, 100Ah)
    
Result: 12V, 200Ah total
```

#### 4. Household Appliances
Refrigerator, TV, microwave all parallel:
```
120V ┌───Fridge
     ├───TV
     └───Microwave

Each can be used independently
```

## Comparison Table

| Characteristic | Series Circuit | Parallel Circuit |
|---------------|----------------|------------------|
| **Current** | Same through all components<br>`I₁ = I₂ = I₃ = Iₜₒₜₐₗ` | Divides among branches<br>`Iₜₒₜₐₗ = I₁ + I₂ + I₃` |
| **Voltage** | Divides among components<br>`Vₜₒₜₐₗ = V₁ + V₂ + V₃` | Same across all components<br>`V₁ = V₂ = V₃ = Vₜₒₜₐₗ` |
| **Resistance** | Total increases (sum)<br>`Rₜₒₜₐₗ = R₁ + R₂ + R₃` | Total decreases (reciprocal sum)<br>`1/Rₜₒₜₐₗ = 1/R₁ + 1/R₂ + 1/R₃` |
| **Component Failure** | Breaks entire circuit<br>Nothing works | Others continue working<br>Only failed component stops |
| **Path for Current** | One single path | Multiple paths |
| **Adding Components** | Increases total resistance | Decreases total resistance |
| **Example Application** | Voltage dividers, safety switches | Home wiring, car lights |

## Visual Comparison

### Series Circuit Example
```
9V Battery, Three 100Ω Resistors

Circuit:
  ⊕ 9V ⊖
  │    │
  R₁ 100Ω  ← 3V drop
  │    │
  R₂ 100Ω  ← 3V drop
  │    │
  R₃ 100Ω  ← 3V drop
  │    │
  └────┘

Current: I = V/R = 9V/300Ω = 0.03A (30mA)
- Same 30mA through all resistors
- Each resistor drops 3V
- Total resistance: 300Ω
```

### Parallel Circuit Example
```
9V Battery, Three 100Ω Resistors

Circuit:
      ⊕ 9V ⊖
  ┌───┴───┬───┬───┐
  R₁      R₂  R₃
  100Ω    100Ω 100Ω
  90mA    90mA 90mA
  │       │   │
  └───┬───┴───┴───┘

Current through each: I = V/R = 9V/100Ω = 0.09A (90mA)
Total current: 90mA + 90mA + 90mA = 270mA
Total resistance: 100Ω/3 = 33.3Ω
- Each resistor sees full 9V
- Current divides: 90mA through each
- Total resistance: 33.3Ω (less than any individual!)
```

## Practical Examples

### Example 1: Series LED Circuit

Calculate resistor needed for LED in series with 9V battery:

```
Circuit:
  ⊕ 9V ⊖
  │    │
  R    ?   ← Current limiting resistor
  │    │
  LED  2V  ← Drops ~2V, needs 20mA
  │    │
  └────┘

Given:
- Battery: 9V
- LED voltage drop: 2V
- LED current needed: 20mA = 0.02A
- Resistor voltage: 9V - 2V = 7V

Solve for R:
R = V / I = 7V / 0.02A = 350Ω

Use 330Ω or 470Ω resistor (standard values)
```

### Example 2: Parallel Resistors for Lower Resistance

You need 50Ω but only have 100Ω resistors. How many in parallel?

```
For two 100Ω resistors:
Rₜₒₜₐₗ = R / n = 100Ω / 2 = 50Ω ✓

Solution: Use two 100Ω resistors in parallel

Circuit:
  ┌──100Ω──┐
──┤        ├──  = 50Ω total
  └──100Ω──┘
```

### Example 3: Home Circuit

Your home has 120V outlets with multiple devices:

```
     120V
  ┌───┴───┬────┬─────┐
  TV      Fan  Lamp
  2A      1A   0.5A
  │       │    │
  └───┬───┴────┴─────┘
      │
    3.5A total

All devices:
- Get full 120V
- Work independently
- Can be turned on/off separately
- Total current: 2A + 1A + 0.5A = 3.5A
```

## Water Flow Analogy

### Series: Single Pipe
```
Tank → │═══│═══│═══│ → Out
       │ 1 │ 2 │ 3 │
       
- Same flow through all sections
- Pressure drops at each section
- Block one → all stops
```

### Parallel: Multiple Pipes
```
       ┌═══════┐
Tank → ├═══════┤ → Out
       └═══════┘
       
- Same pressure in all pipes
- Flow divides among pipes
- Block one → others still flow
```

## Common Mistakes to Avoid

### Mistake 1: Confusing Voltage Distribution
❌ **Wrong**: "Parallel circuits divide voltage"  
✅ **Correct**: "Series circuits divide voltage; parallel circuits have same voltage everywhere"

### Mistake 2: Adding Parallel Resistances Incorrectly
❌ **Wrong**: `Rₜₒₜₐₗ = R₁ + R₂` (series formula)  
✅ **Correct**: `1/Rₜₒₜₐₗ = 1/R₁ + 1/R₂` (parallel formula)

### Mistake 3: Assuming Current is Same in Parallel
❌ **Wrong**: "All parallel branches have same current"  
✅ **Correct**: "All parallel branches have same voltage; current depends on each branch's resistance"

## Mixed Circuits (Series-Parallel)

Real circuits often combine both:

```
Example:
        ┌──R₂──┐
  ──R₁──┤      ├──R₄──
        └──R₃──┘

R₁ and R₄: Series with the parallel group
R₂ and R₃: Parallel with each other

Solve step by step:
1. Calculate parallel section (R₂∥R₃)
2. Add series resistances (R₁ + R₂∥R₃ + R₄)
```

## Real-World Considerations

### Series Circuits
✅ **Advantages:**
- Simple design
- Same current everywhere (easy to predict)
- Good for voltage division

❌ **Disadvantages:**
- One failure breaks everything
- Can't control components independently
- Difficult to add/remove components

### Parallel Circuits
✅ **Advantages:**
- Components work independently
- Failure of one doesn't affect others
- Easy to add/remove components
- Each component gets full voltage

❌ **Disadvantages:**
- Higher total current (thicker wires needed)
- More complex to analyze
- Can overload power source if too many branches

## Key Takeaways

### Series Circuits
✅ **Current** is the same everywhere  
✅ **Voltage** divides among components  
✅ **Resistance** increases (adds up)  
✅ One failure **breaks entire circuit**  
✅ Used for: voltage dividers, safety switches, current limiting

### Parallel Circuits
✅ **Voltage** is the same everywhere  
✅ **Current** divides among branches  
✅ **Resistance** decreases (reciprocal sum)  
✅ Components work **independently**  
✅ Used for: home wiring, car lights, battery banks

### Quick Memory Aid
**"Same Same Divides"**
- **Series**: **Same** current, divides voltage
- **Parallel**: **Same** voltage, divides current

## What's Next?

You now understand how components can be connected in series and parallel! These concepts are fundamental to circuit design and analysis. You'll use them constantly when building and troubleshooting circuits.

➡️ Review the chapter concepts in [11-summary-and-practice.md](./11-summary-and-practice.md)
