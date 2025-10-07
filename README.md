# Place and Route Flow 

This repository documents my end-to-end ASIC Physical Design Flow project implemented using Synopsys EDA tools (Design Compiler, ICC2, PrimeTime).
---

##  Project Overview  
- **Objective**: Complete **Place & Route implementation** for a synthesized design.  
- **Design**: `ChipTop` module with 61K standard cells and 40 macros.  
- **Target Frequency**: 434 MHz (2.3 ns clock period).  
- **PnR Flow Steps**:  
  1. Floorplanning (**ICC2**) – die size, macro & IO port placement, Voltage area creation,power planning  
  2. Placement (**ICC2**) – standard cell placement & congestion optimization  
  3. Clock Tree Synthesis (CTS) – clock skew & latency balancing  
  4. Routing – global & detailed routing, DRC fixes 
  5. Post-Route Optimization – timing fixes, buffering, crosstalk 
  6. Signoff (**PrimeTime**) – STA, power, DRC/LVS checks  
  7. GDSII Generation – final tape-out layout
---

## Tools
| Stage                | Tool                | Purpose                                |
| -------------------- | ------------------- | -------------------------------------- |
| Synthesis            | **Design Compiler** | RTL to gate-level netlist              |
| Place & Route        | **ICC2**            | Floorplanning, Placement, CTS, Routing |
| Timing Analysis      | **PrimeTime**       | Signoff STA                            |
| Parasitic Extraction | **StarRC**          | SPEF generation                        |

---
## License

This project is licensed under the MIT License.

---
![Project](https://img.shields.io/badge/Project-PD_Flow-blue?style=for-the-badge)
![Tools](https://img.shields.io/badge/Tools-DC_|_ICC2_|_STARRC_|_PrimeTime-limegreen?style=for-the-badge)
![Macros](https://img.shields.io/badge/Macros-40-red?style=for-the-badge)
![Std_Cells](https://img.shields.io/badge/Std_Cells-52K-blue?style=for-the-badge)
![Frequency](https://img.shields.io/badge/Frequency-434MHz-red?style=for-the-badge)
![Utilization](https://img.shields.io/badge/Utilization-75%25-orange?style=for-the-badge)
![Hold_WNS](https://img.shields.io/badge/Hold_WNS-0.05ns-blue?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-gold?style=for-the-badge)


