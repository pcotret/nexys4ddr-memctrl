:santa:
# nexys4ddr-memctrl
The goal of this repository is to generate a proper external memory controller for the [Nexys4 DDR board](https://reference.digilentinc.com/reference/programmable-logic/nexys-4-ddr/start)
- [Nexys 4 DDR Xilinx MIG Project](https://reference.digilentinc.com/reference/programmable-logic/nexys-4-ddr/start)
  - Files to configure the MIG wizard.
  - Stated to work with ISE 14.7.
  - Doesn't work with Vivado 2018.2 nor Vivado 2019.2
## Vivado test
As MIG files are not understood by the MIG wizard, I'll try to manually generate a MIG. Problem #1 : some parameters in the `.prj` file do not have the same values/options. Default generation failed, here is a partial log:
```
set_property -name {CONFIG.XML_INPUT_FILE} -value  {mig_a.prj} -objects [get_bd_cells mig_7series_0]
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
ERROR: [Ip 78-140] conversion to double from string is failed
INFO: [Common 17-14] Message 'Ip 78-140' appears 100 times and further instances of the messages will be disabled. Use the Tcl command set_msg_config to change the current settings.
vector::_M_range_check: __n (which is 0) >= this->size() (which is 0)
ERROR: [IP_Flow 19-3475] Tcl error in ::ipgui_design_1_mig_7series_0_0::updateAllModelParams procedure for BD Cell 'mig_7series_0'. vector::_M_range_check: __n (which is 0) >= this->size() (which is 0)
INFO: [IP_Flow 19-3438] Customization errors found on 'mig_7series_0'. Restoring to previous valid configuration.
ERROR: [BD 41-245] set_property error - Customization errors found on 'mig_7series_0'. Restoring to previous valid configuration.
ERROR: [Common 17-39] 'set_property' failed due to earlier errors.
```
