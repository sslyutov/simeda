Sergey Slyutov
January 15, 2026

Requered parts
1. Raspberry Pi
2. Set of resistors




Simulation of EDA load

Schematic for 1–24 µS (42kΩ – 1MΩ)
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
