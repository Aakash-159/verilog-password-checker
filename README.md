# verilog-password-checker
This Real-Time Password Checker project is a simple Verilog design that verifies a fixed-length password entered character-by-character in real-time. The password is hardcoded as "1234" (ASCII codes). The module continuously checks the input characters on each clock cycle and asserts a match signal when the correct password sequence is entered.
# Real-Time Password Checker in Verilog

A simple Verilog project for checking a 4-character password in real-time, with testbench for simulation. This is ideal for FPGA or ASIC beginner projects.

---

## Project Description

This project implements a **password checker** in Verilog that verifies a password sequence character-by-character. The correct password is hardcoded as `"1234"` (ASCII). 

**Features:**

- Real-time password input
- Password validation on the fly
- Synchronous reset
- Testbench included for simulation

---

## Files

- `password_checker.v` — The main password checking module
- `tb_password_checker.v` — Testbench to verify functionality

---

## Usage

### Simulation

You can simulate this design using Icarus Verilog:

```bash
iverilog -o password_checker_tb.vvp password_checker.v tb_password_checker.v
vvp password_checker_tb.vvp
