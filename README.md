:santa:
# nexys4ddr-memctrl
The goal of this repository is to generate a proper external memory controller for the [Nexys4DDR board](https://reference.digilentinc.com/reference/programmable-logic/nexys-4-ddr/start)
- [Nexys 4 DDR Xilinx MIG Project](https://reference.digilentinc.com/reference/programmable-logic/nexys-4-ddr/start)
  - Files to configure the MIG wizard.
  - Stated to work with ISE 14.7.
  - Doesn't work with Vivado 2018.2 nor Vivado 2019.2
## Vivado test
As MIG files are not understood by the MIG wizard, I'll try to manually generate a MIG. Problem #1 : some parameters in the `.prj` file do not have the same values/options.
