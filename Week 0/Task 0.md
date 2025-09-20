# ASIC/SoC Design Flow Documentation

## Stages Overview

| Stage            | Description                                | Verification     | Key Artifacts                    |
|------------------|--------------------------------------------|------------------|-----------------------------------|
| O0/O1 Specification | Functional modeling using C (Specs, GCC)  | C language testbench | C model, GCC results               |
| O2 RTL Architecture | Hardware described in Verilog (RTL)       | RTL/C comparison    | Processor, Peripherals, Macros, Analog IPs |
| O3 SoC Integration | Assembling IPs into complete SoC           | Module integration | Integrated SoC                     |
| O4 Physical & Application | Floorplanning, routing, DRC/LVS, Deployment | Silicon verification | GDSII, Product deployment          |

## End Applications

- Smartwatches (iwatch)
- Arduino development boards
- Consumer electronics (TV panels)
- Home appliance control (AC applications)

## Design Principle

At every stage (O0 → O1 → O2 → O3 → O4) functional equivalence is ensured, validated by testbenches and post-fabrication testing for reliable deployment.
