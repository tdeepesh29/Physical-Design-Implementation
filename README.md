# Place and Route Flow 🚀

This repository documents my end-to-end ASIC Physical Design Flow project implemented using Synopsys EDA tools (Design Compiler, ICC2, PrimeTime).
---

## 🚀 Project Overview  
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

## 🛠️ Tools
- **Synthesis**: Design Compiler  
- **PnR**: Synopsys ICC2  
- **Timing Analysis**: PrimeTime  
- **SPEF Extraction**: STARRC 
---
## 📄 License

This project is licensed under the MIT License.


