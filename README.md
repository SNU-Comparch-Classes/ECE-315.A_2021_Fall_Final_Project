# ECE-315.A_2021_Fall_Final_Project

This repo is for announcements and documents

## FIXME
- For `build/layer_tb`, fix the device as below
  - `Settings` -> `General` -> `Project Device` -> `Parts` -> "xc7a100tcsg324-1" (neither Arty-A7 100T nor Nexys-A7 100T)
- Testbench IP path issue
  - Solution: Replace `build/layer_tb` with `layer_tb` in `patch`
  - For the new `layer_tb`, the data files (txt) are not included in the xpr file. So, you need to manually add them to the `Simulation Sources` via `Add or create simulation sources`. Once they are added, they will be placed under `Text` in `Simulation Sources`.
    - (11/28 01:33) updated: the data files are included for `layer_tb`
