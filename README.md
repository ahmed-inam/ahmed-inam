## Ahmed Inam Chowdhury

Computer engineering at Purdue. I build processors, and the instruments that
decide whether they actually work.

Most of my time goes to RTL and verification. The design is the shorter half —
the longer half is finding out what you have really proved, which is usually
less than the green result suggests.

---

### Projects

**[RV32IM](https://github.com/ahmed-inam/RV32IM)** — a dual-core, two-wide
out-of-order RISC-V processor with a UVM verification environment.
Two harts, speculative execution, private L1s kept coherent with MESI over an
AXI4 crossbar, LR/SC atomics and a CLINT. ~9,700 lines of SystemVerilog, checked
instruction-by-instruction against Spike across ~189,000 instructions, with 757
coverage bins and mutation testing behind the result. Written from nothing over
seven stages. Start with [`docs/overview.pdf`](https://github.com/ahmed-inam/RV32IM/blob/main/docs/overview.pdf).

**[AXI4](https://github.com/ahmed-inam/AXI4)** — a synthesizable 2×2 AXI4
crossbar. Full five-channel signalling, bursts, multiple outstanding
transactions, ID-based response routing and DECERR, with two independent
testbench flows and an RTL-side protocol checker.

**[Async-FIFO](https://github.com/ahmed-inam/Async-FIFO)** — a parameterized
dual-clock FIFO. Gray-coded pointers across two-flop synchronizers in the
partitioned Cummings style, with a class-based testbench covering reset,
full/empty boundaries, concurrent access and asymmetric clock ratios.

**[sat-solver](https://github.com/ahmed-inam/sat-solver)** — a conflict-driven
clause-learning SAT solver in C++17. Single file, no dependencies, Glucose-class
heuristics over an arena allocator. Verifies its own model before printing it.

---

### What I work in

SystemVerilog · UVM · RISC-V · computer architecture · cache coherence ·
constrained-random and coverage-driven verification · C++ · Python ·
Verilator, Vivado/XSim, Spike

**chowdh48@purdue.edu**
