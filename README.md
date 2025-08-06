# 4-to-1 MUX Using 2-to-1 MUX in Verilog

This project demonstrates the hierarchical structural design of a 4-to-1 multiplexer using basic 2-to-1 multiplexer modules in Verilog HDL. The 4:1 MUX is constructed using three 2:1 MUXes to illustrate modular design principles and promote reusability in hardware description. The design is verified using a testbench and simulated on EDA Playground. This project showcases digital logic design, behavioral simulation, and fundamental principles of hardware modularity.

## 🧠 Logic Overview

A 4-to-1 MUX selects one of 4 input lines based on a 2-bit select signal. You can implement it using **three 2-to-1 MUXes**:
- MUX1 selects between `in[0]` and `in[1]`
- MUX2 selects between `in[2]` and `in[3]`
- MUX3 selects between the outputs of MUX1 and MUX2

## 📎 Files

- `4to1mux_using_2to1mux.sv` – 4:1 MUX built using three 2:1 MUXes
- `4to1_mux_tb.sv` – Testbench for simulating the 4:1 MUX
- `4to1_MUX_waveform.png` – 4to1 MUX Waveform Screenshot 

## ▶️ Run Simulation

This project was created and tested on **EDA Playground**.

### 🧪 Simulation Output

| Time (ns) | Sel | Inputs | Y |
|-----------|-----|--------|---|
| 0         | 00  | 1010   | 0 |
| 10        | 01  | 1010   | 1 |
| 20        | 10  | 1010   | 0 |
| 30        | 11  | 1010   | 1 |


