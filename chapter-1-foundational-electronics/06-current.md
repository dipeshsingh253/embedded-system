# Current

## What Is Current?

**Current** is the flow of electrons through a conductor. When electrons move through a wire or component, we say current is flowing.

Think of it like water flowing through a pipe—current is the electrical equivalent of flow rate.

> **Current = Flow of Electrons**

## The Unit: Amperes (A)

Current is measured in **Amperes** (often shortened to **Amps**), abbreviated as **A**.

Named after André-Marie Ampère, a pioneer in electromagnetism.

### What Is One Ampere?

One ampere means **6.24 × 10¹⁸ electrons** flowing past a point every second!

That's:
- 6,240,000,000,000,000,000 electrons per second
- About 6 quintillion electrons per second

In practical terms: 1 Ampere = 1 Coulomb of charge per second

Where 1 Coulomb is the total charge of those 6.24 × 10¹⁸ electrons.

**Formula:**
```
I = Q / t
```
- I = Current (Amperes)
- Q = Charge (Coulombs)
- t = Time (seconds)

## Current Flows Through Components

This is important: **Current flows THROUGH things.**

- Voltage is measured **BETWEEN** two points
- Current is measured **THROUGH** a component or wire

```
     Voltage               Current
     (across)              (through)
        ↓                     ↓
    A ─────── B          ────⟶────
      V = ?                I = ?
      
   "Voltage                "Current
    between                through
    A and B"               the wire"
```

## Common Current Examples

| Device/Application | Current |
|-------------------|---------|
| LED (small) | 20 mA (0.02 A) |
| USB charging | 500 mA - 2 A |
| Phone charger | 1 - 2 A |
| Laptop | 3 - 5 A |
| Light bulb (60W) | 0.5 A |
| Microwave | 10 - 15 A |
| House circuit breaker | 15 - 20 A (max) |
| Car starter | 100 - 200 A |
| Lightning strike | 20,000 - 200,000 A |

Notice that we use different scales:
- **mA (milliamperes)** = 0.001 A = 1/1000 A
- Common for small electronics
- **A (amperes)** = base unit
- Common for household devices

## Conventional Current vs Electron Flow

This is a quirk of history that confuses many beginners:

### Electron Flow (Reality)
```
  ⊖ Negative          Positive ⊕
    (-) ────────────────────→ (+)
        Electrons actually flow
```

**Reality**: Electrons flow from **negative to positive** (because electrons are negatively charged and are repelled by negative, attracted to positive).

### Conventional Current (Convention)
```
  ⊖ Negative          Positive ⊕
    (-) ←──────────────────── (+)
        "Current" direction
```

**Convention**: We say current flows from **positive to negative**.

### Why the Difference?

Benjamin Franklin (1700s) guessed that current was a flow of positive charge from + to -. He had a 50/50 chance and guessed wrong! Later, scientists discovered electrons (negative) actually flow the opposite way.

But by then, all the conventions, formulas, and notation were established. Rather than rewrite everything, we kept the convention.

### What Should You Use?

**Use conventional current** (+ to -) when:
- Drawing circuit diagrams
- Analyzing circuits
- Following textbooks and datasheets
- Communicating with other engineers

**Think about electron flow** (- to +) when:
- Understanding what's physically happening
- Learning the fundamentals

In this guide, we'll primarily use **conventional current** (+ to -) for circuit analysis, but we'll remind you that electrons actually move the opposite way.

## Water Flow Analogy

Current is exactly like water flowing through a pipe:

### Water System
```
    Tank            
   ┌─────┐         
   │     │         
   │ ▓▓▓ │         
   └──┬──┘         
      │            
   ┌──▼──┐         
   │ PIPE │  ← Water flows
   └─────┘         
      
   Flow rate: 5 liters/second
```

### Electrical System
```
   Battery
    ⊖   ⊕
    │   │
    ├───┤
    │ ─ │  ← Electrons flow
    └───┘
    
   Current: 5 Amperes
```

### The Analogy

| Water System | Electrical System |
|-------------|-------------------|
| Water flow rate (liters/sec) | Current (Amperes) |
| Pipe | Wire |
| Water molecules | Electrons |
| Pump | Battery |
| Open valve | Closed switch |
| Closed valve | Open switch |

## Current Needs Voltage AND a Complete Path

For current to flow, you need TWO things:

### 1. Voltage (Pressure)
Without voltage, there's no push to make electrons flow.

```
    No battery
    
    ────────────────
    
    Current: 0 A (no flow)
```

### 2. Complete Circuit (Path)
Even with voltage, electrons need a complete path from - to +.

```
    With battery, but broken wire:
    
    ⊖ ─────  X  ───── ⊕
           Gap
    
    Current: 0 A (no complete path)
```

### Both Together
```
    Complete circuit:
    
    ⊖ ──────────────⊕
    │              │
    └──────────────┘
    
    Current flows! ✓
```

## Current Is the Same Everywhere in a Series Circuit

This is counterintuitive for many beginners:

In a simple series circuit, **the current is the same at every point**.

```
       ⊖ Battery ⊕
        │       │
    I=2A│       │I=2A
        │       │
       💡 LED  
        │
    I=2A│
        │
        └───────┘
```

Think of water in a pipe:
- If 5 liters/second enters one end
- Then 5 liters/second must exit the other end
- Water doesn't pile up or disappear in the middle
- Same flow rate everywhere

Similarly with electrons:
- Electrons flowing into LED = Electrons flowing out
- No electrons pile up inside components
- Same current everywhere in the loop

## Measuring Current

To measure current, we use an **ammeter** (or multimeter in current mode):

**Important**: To measure current, you must **break the circuit** and insert the meter **in series**:

```
Before (measuring voltage):
   Battery
    ⊖  ⊕
    │  │
    └─💡─┘

Measuring current:
   Battery
    ⊖  ⊕
    │  │
    │ ┌─────┐
    └─┤  A  ├─💡
      └─────┘
      Ammeter inserted
      in series
```

Never connect an ammeter in parallel (across a battery)—it will short circuit!

## Current and Safety

Current is what actually hurts you, not voltage:

### Danger Levels

| Current | Effect |
|---------|--------|
| < 1 mA | Not felt |
| 1 - 5 mA | Slight tingle |
| 5 - 10 mA | Painful shock |
| 10 - 20 mA | Muscle contractions |
| 20 - 50 mA | Difficulty breathing |
| 50 - 100 mA | Possible heart fibrillation |
| > 100 mA | Likely fatal |

⚠️ **Safety**: Even small currents (> 10 mA) through your body can be dangerous. Always be careful with electricity!

Note: It takes voltage to push current through your body's resistance. Low voltage (like 5V) typically can't push dangerous current through dry skin.

## Key Takeaways

✅ **Current is the flow of electrons** through a conductor

✅ Unit: **Amperes (A)**, often milliamperes (mA) for small currents

✅ 1 A = about 6.24 × 10¹⁸ electrons per second

✅ Current flows **THROUGH** components (voltage is ACROSS)

✅ **Conventional current**: + to - (used in circuit analysis)

✅ **Electron flow**: - to + (physical reality)

✅ Like **water flow rate** through a pipe

✅ Needs **voltage AND complete path** to flow

✅ Current is the **same everywhere** in a series circuit

✅ Measured with ammeter **in series** (breaking the circuit)

✅ Current through body can be **dangerous** (> 10 mA)

## What's Next?

You now understand voltage (pressure) and current (flow). But there's one more fundamental concept: what opposes the flow? What makes it harder for current to flow?

➡️ Continue to [07-resistance.md](./07-resistance.md)
