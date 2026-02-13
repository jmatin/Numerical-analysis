# 🌊 Numerical Simulation on a Wavy Surface

Numerical analysis project (INFO-F-205, 2022) — Simulation of a body rolling on an undulated surface using the explicit Euler method, based on mechanical energy conservation.

## 📋 Description

This project simulates the motion of a body (or wheel) on a wavy surface defined by:


$$
f(x) = \frac{\cos(3\pi x^2) \cdot (1 - x - x^2)}{10}
$$


The motion is governed by an ODE derived from energy conservation (kinetic + potential), solved numerically using the **explicit Euler method**.

### Key features:
- Explicit Euler method with direction handling
- Forbidden zone detection (|ẋ|² < 0)
- Zero-velocity restart via acceleration
- Energy conservation analysis (E_cin, E_pot, E_tot)
- Time-step sensitivity study (h vs h×100)

## 📁 Project Structure
```
├── README.md
├── doc/
│ ├── projet2022infoF205.pdf # Project assignment
│ └── numerical_analysis (1).pdf # Report
├── src/
│ ├── roadprofile.m # Road profile f(x) and f'(x)
│ └── projet2022INFOF205.m # Main simulation script
```
