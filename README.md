# Matrix Multiplier VLSI Architectures

Comparative analysis of three hardware architectures for NxN square matrix multiplication, implemented in Verilog HDL and synthesized using Cadence Genus.

## Architectures

**Serial** — Single MAC unit with FSM control. Lowest area and power, but requires N³+N² clock cycles.

**Pipelined** — N² multipliers with pipeline registers and accumulator. Balanced trade-off, produces result every N cycles.

**Parallel** — N³ multipliers computing all products simultaneously. Single-cycle output but highest area and power.

## Matrix Sizes

Each architecture is parameterized and tested for 2×2, 3×3, and 4×4 matrices with 4-bit elements.

## Tools Used

- Cadence NCLaunch/SimVision (simulation)
- Cadence Genus (synthesis)
- Cadence Innovus (physical design)
