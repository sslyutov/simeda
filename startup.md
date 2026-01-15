# Simulation of EDA Load

**Sergey Slyutov**  
**January 15, 2026**

---

## Required Parts

1. Raspberry Pi
2. Set of resistors:
   - 47kΩ (1%)
   - 68kΩ (1%)
   - 100kΩ (1%)
   - 150kΩ (1%)
   - 220kΩ (1%)
   - 330kΩ (1%)
   - 470kΩ (1%)
   - 1MΩ (1%)

---

## Schematic for 1–24 µS (42kΩ – 1MΩ)

```
                            RASPBERRY PI
                       ┌─────────────────────┐
                       │                     │
                       │  GPIO17 (pin 11) ───┼──── 47kΩ ────┐
                       │  GPIO27 (pin 13) ───┼──── 68kΩ ────┤
                       │  GPIO22 (pin 15) ───┼──── 100kΩ ───┤
                       │  GPIO23 (pin 16) ───┼──── 150kΩ ───┤
                       │  GPIO24 (pin 18) ───┼──── 220kΩ ───┼───► LOAD +
                       │  GPIO25 (pin 22) ───┼──── 330kΩ ───┤
                       │  GPIO5  (pin 29) ───┼──── 470kΩ ───┤
                       │  GPIO6  (pin 31) ───┼──── 1MΩ ─────┘
                       │                     │
                       │  GND (pin 6) ───────┼─────────────────► LOAD -
                       │                     │
                       └─────────────────────┘
```

---

## Resistor Values

| GPIO | Pin | Resistor | Conductance |
|------|-----|----------|-------------|
| 17   | 11  | 47kΩ     | 21.3 µS     |
| 27   | 13  | 68kΩ     | 14.7 µS     |
| 22   | 15  | 100kΩ    | 10.0 µS     |
| 23   | 16  | 150kΩ    | 6.7 µS      |
| 24   | 18  | 220kΩ    | 4.5 µS      |
| 25   | 22  | 330kΩ    | 3.0 µS      |
| 5    | 29  | 470kΩ    | 2.1 µS      |
| 6    | 31  | 1MΩ      | 1.0 µS      |
