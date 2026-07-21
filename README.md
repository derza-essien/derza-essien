# Denzil Erza-Essien

I am an Electronic and Computer Engineering Student at Imperial College London who focuses on FPGA-focused acceleration and low-latency systems.

My projects, and general focus mainly consist of performance optimisation in both hardware and software systems. I prefer projects where I am more involved on the hardware side optimising speedup/throughput multiples.

---

## Projects


The following table details the projects I have contributed to. Unfortunately, some of these projects require private repositories for security reasons. This table should give a clear indication of my project contributions with a summary of my role in them.

| Project | Role | Tools | Summary |
| - | - | - | - |
| [NASDAQ-ITCH Feed Handler](https://github.com/an-thony350/ITCH-Feed-Handler-and-Order-Book) | Contributer to Hardware & Software design & Verification | SystemVerilog, PYNQZ1, Xilinx Vivado, Python | Contributed to the overall hardware design, verifying rtl I designed as well as contibuting to the python scripts simulating order-book data |
| [Fractal Viewer & Mathematical Accelerator](https://github.com/an-thony350/FractalScope) | Hardware Design Lead & Low-latency Software Lead | SystemVerilog, Verilog, PYNQZ1, Xilinx Vivado, C++, Python | Co-designed the RTL for all releases of the fractal set viewer & designed the cpu baseline to compare throughput multiples between software & hardware |
| [FPGA-Accelerated HFT System](https://github.com/Information-Processing/trading_indicators) | Hardware Design Lead | SystemVerilog, PYNQZ1, Xilinx Vivado | Designed the RTL for the fixed-point matrix multiplier for a linear regression model |
| [C90 Compiler](https://github.com/derza-essien/C90-Compiler) | Contributer | C++, RISC-V Assembly, Yacc | Designed the parser forming the AST tree and co-designed the code generation sections which call functions relative to tree position |
| [Chat bot](https://github.com/Information-Processing/chat-bot) | Hardware Design Lead | SystemVerilog, Verilog, PYNQZ1, Xilnx Vivado | Designed the RTL allowing for speach inputs through the board microphone as well as noise-reduced (i.e. high signal-to-noise ratio) speaker outputs |
| [RISC-V Processor](https://github.com/aa4923/RISC-V22) | Team Lead | SystemVerilog, C++, Verilator, RISC-V Assembly | Lead the design & verification of a 5-stage pipelined RV32I RISC-V processor |

---

## Contributions

The list below explains what some of the prior mentioned projects consist of, as well as more information my specific contributions, as well as their impacts.

### NASDAQ-ITCH Feed Handler

A low-latency feed handler, implemented via the Nasdaq TotalView-ITCH 5.0 specifcation. Also includes an Order & Price book tracking bid & ask prices.

- Designed data handler & order book logic, allowing for micro-second price management
- Tested with historical Nasdaq-ITCH data using the 5.0 specification
- Verification through systemverilog, and verilator (via cocotb) testbenches, with comparison to a golden model

### Fractal Viewer & Mathematical Accelerator

An interactive HDMI display of fractal sets, with educational displays exlpaining the mathematics behind the fractal sets.

- 23-cored parallelised design computing Q4.22 numbers in a 7-stage iterative pipeline
- 96.36% DSP utilisation with LUT & FF utilisation both under 80%
- ~53x Throughput speedup relative to a multithreaded CPU baseline

### FPGA-Accelerated HFT System

An FPGA-Accelerated system tracking Crypto markets, accelerated and controlled through a linear regression model updated on the FPGA.

- Computed matrix multiplication for the linear regression model through outer-product accumulation in a 1-cycle pipeline
- Converted IEEE-754 floating-point data into fixed-point data (avoidig congestion) with a negligible, mean 0.5% quantization error
- Maintained an average speedup of ~18x, with a peak speedup of ~68x
- Implemented voice interaction of system, allowing for switching of market and leverage

### C90 Compiler

A Compiler (made with mostly C++) which converts to RISC-V assembly.

- Parsing through AST trees done in Yacc which calls code gen functions in C++
- Tested with ~200 tests passing each one, each covering uniquely written features

### RISC-V Processor

A 5-stage RISC-V core complete with forwarding, hazard detection, and branch prediction.

- Implemented a 2-way set associaive cache block with a LRU replacement policy

---

## Skills

**Software:** C++, C, Python, RISC-V Assembly

**Hardware:** SystemVerilog, Verilog

**Tools:** Xilinx Vivado, Linux, Git, Pynq

