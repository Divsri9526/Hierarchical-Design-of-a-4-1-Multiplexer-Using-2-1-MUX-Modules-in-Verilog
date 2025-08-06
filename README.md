# 4-to-1 MUX Using 2-to-1 MUX in Verilog (EDA Playground)

This project demonstrates how a 4-to-1 multiplexer can be constructed using only 2-to-1 multiplexers in **Verilog HDL**, simulated using **EDA Playground**.

## 🧠 Logic Overview

A 4-to-1 MUX selects one of 4 input lines based on a 2-bit select signal. You can implement it using **three 2-to-1 MUXes**:
- MUX1 selects between `in[0]` and `in[1]`
- MUX2 selects between `in[2]` and `in[3]`
- MUX3 selects between the outputs of MUX1 and MUX2

    in[0] ----\
               MUX1 --\
    in[1] ----/        \
                         MUX3 ----> y
    in[2] ----\        /
               MUX2 --/
    in[3] ----/


## 📎 Files

- `mux4to1_using_2to1.v` – 4:1 MUX built using three 2:1 MUXes
- `mux4to1_tb.v` – Testbench for simulating the 4:1 MUX

## ▶️ Run Simulation

This project was created and tested on **EDA Playground**.

## 🧪 Sample Output

Time Sel Inputs Y
0    00  1010   0
10   01  1010   1
20   10  1010   0
30   11  1010   1

