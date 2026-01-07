# AXI-Stream Learning Project (Verilog RTL)

This repository contains a **minimal, educational implementation of an AXI-Stream–style data transfer system** written in Verilog.  
The purpose of this project is to **understand the fundamentals of AXI-Stream communication**, including handshaking, back-pressure, and packetized data transfer using FSM-based control.

⚠️ **Note:** This is **not a fully AXI-Stream compliant IP core**. It is intentionally simplified for learning and demonstration purposes.

---

## 🎯 Objectives

- Learn the AXI-Stream `TVALID` / `TREADY` handshake
- Understand back-pressure in streaming systems
- Implement packetized data transfer using `TLAST`
- Design FSM-controlled streaming logic in RTL
- Simulate end-to-end streaming between master and slave

---

## 📁 Repository Structure

```text
axi-stream-learning/
│
├── rtl/
│   ├── axis_m.v        # AXI-Stream Master (data source)
│   ├── axis_s.v        # AXI-Stream Slave (data sink)
│   └── top.v           # Top-level integration
│
├── sim/
│   ├── tb_axis_stream.v   # Testbench (optional / recommended)
│   └── waveforms.png      # Simulation waveform screenshots
│
├── docs/
│   ├── master_fsm.png
│   ├── slave_fsm.png
│   └── timing_diagram.png
│
├── README.md
└── LICENSE
