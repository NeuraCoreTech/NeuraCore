# NeuraCore

Open FPGA-based Edge AI and CNN Acceleration Platform.

NeuraCore is a custom Zynq-7000 SoC FPGA platform designed for exploring hardware-accelerated machine learning inference and Edge AI deployment.

The platform combines:
- a custom FPGA development board
- CNN accelerator RTL
- Linux middleware
- TensorFlow Lite integration
- hardware/software co-design workflows

into a unified open platform for AI acceleration research, experimentation, and deployment.

The current demonstration workload focuses on OCR inference deployment as an end-to-end validation of the platform.



---

## Vision

Modern AI education and experimentation are increasingly dependent on expensive GPUs, cloud subscriptions, and closed ecosystems.

NeuraCore aims to provide:
- an accessible AI experimentation platform
- hardware-aware ML education
- FPGA accelerator exploration
- open hardware + open RTL infrastructure
- end-to-end Edge AI deployment workflows

The platform is designed so beginners can use high-level Python/TFLite APIs, while advanced users can directly develop RTL accelerators and deploy custom hardware architectures.

---
## Demonstration Workload

The current reference deployment targets OCR inference acceleration on FPGA hardware.

The OCR pipeline is used as a practical demonstration of:
- model deployment
- quantized inference
- DMA-based data movement
- accelerator integration
- PS-PL communication
- real-time Edge AI execution

while the underlying accelerator architecture is designed to support broader CNN workloads.

---

## Platform Overview

NeuraCore consists of three tightly integrated layers:

### Hardware Layer
Custom FPGA SoC development board based on:
- Xilinx Zynq-7000
- ARM Processing System (PS)
- FPGA Programmable Logic (PL)

### Middleware Layer
- PetaLinux
- AXI DMA infrastructure
- Hardware abstraction layer
- Custom drivers

### Software Layer
- TensorFlow Lite integration
- Quantized inference support
- Python APIs
- Profiling and telemetry tools

---

## Core Components

| Component | Description |
|---|---|
| FPGA Board | Custom Zynq-7000 development board |
| AI Accelerator | FPGA-based systolic accelerator |
| Runtime Stack | PetaLinux + TFLite |
| Toolchain | Vivado / Vitis |
| Deployment | Edge AI inference |

---

## Accelerator Architecture

The accelerator architecture explores:
- systolic compute organizations
- spatial dataflow architectures
- memory reuse optimization
- configurable precision arithmetic
- FPGA-oriented accelerator design

The current design direction is inspired by multiple research architectures including:
- Eyeriss
- DianNao
- TPU
- Xilinx DPU
- Angel-Eye
- Cerebras systems

while remaining an independent experimental implementation.

---

## FPGA Board

The custom development board includes:
- Xilinx XC7Z020 SoC
- DDR3L memory subsystem
- Gigabit Ethernet
- USB OTG
- FT2232 JTAG/UART
- QSPI boot flash
- PL expansion IO

---

## Design Goals

- Accessible AI hardware experimentation
- Hardware/software co-design education
- Efficient Edge AI inference
- Open and extensible architecture
- FPGA accelerator research platform
- Low-cost deployment

---

## Development Status

Current status:
- PCB design is done and in in process of ordering for trials
- Accelerator RTL under development
- Bring-up infrastructure planned
- Software integration in progress

---

## Acknowledgements

### Hardware References
The FPGA board design is heavily based on and adapted from the open-source work by rehsd:

https://github.com/rehsd/FPGA

### Research References
The accelerator architecture direction was influenced by research works including:
- Eyeriss
- DianNao
- TPU architectures
- Angel-Eye
- Cerebras systems
- foundational systolic array research

The project direction also benefited from architectural discussions and guidance from Prof. Rajesh Kedia during independent exploration alongside the ESDP Lab course framework.

---

## Disclaimer

This project is intended for research, experimentation, and educational purposes.

The accelerator architecture is inspired by multiple published research works and is not an official implementation of any referenced architecture.

---
