# ECE-315.A_2021_Fall_Final_Project

This repo is for announcements and documents

## FIXME
- For `build/layer_tb`, fix the device as below
  - `Settings` -> `General` -> `Project Device` -> `Parts` -> "xc7a100tcsg324-1" (neither Arty-A7 100T nor Nexys-A7 100T)
- Testbench IP path issue
  - Solution: Replace `build/layer_tb` with `layer_tb` in `patch`
  - For the new `layer_tb`, the data files (txt) are not included in the xpr file. So, you need to manually add them to the `Simulation Sources` via `Add or create simulation sources`. Once they are added, they will be placed under `Text` in `Simulation Sources`.
    - (11/28 01:33) updated: the data files are included for `layer_tb`
- For `Nexys` branch, please update `src/common_ip/mig_dram/mig.prj` to `src/ddr2-mig/mig.prj`.
  - In addition, remove all ports named `ddr2_reset_n`

## Resources
For the questions on VDMA, you can find most of the answers in the document below. Please try to find the information in the document before asking any questions.
- VDMA 6.3: https://www.xilinx.com/support/documentation/ip_documentation/axi_vdma/v6_3/pg020_axi_vdma.pdf
- XC7A100T
  - Overview: https://www.xilinx.com/support/documentation/data_sheets/ds180_7Series_Overview.pdf
  - CLB: https://www.xilinx.com/support/documentation/user_guides/ug474_7Series_CLB.pdf
