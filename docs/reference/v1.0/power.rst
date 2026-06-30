Power Distribution
##################

LimeFEA mPCIe board power delivery network consists of different power rails with different regulators, voltages and filters. LimeFEA mPCIe board power distribution block diagram is presented in 6.

.. figure:: /images/LimeFEA-mPCIe_v1.0_power.svg
  :width: 600

  Figure 6: LimeFEA mPCIe v1.0 power distribution block diagram

LimeFEA mPCIe board may be supplied from USB microB port (USB 5V), PCIe edge connector (12V and 3.3V) or header (3.3V or 5V). It is important to note that only 3.3V is permitted by mPCIe specification, so use 5V power only if manufacturer specifies 5V supply (for example  LimeSDR XTRX does allow 5V power supply voltage):

  * PCIe edge is prefered way to supply power for the LimeFEA mPCIe board. Make sure J2 jumper is placed between +3.3VPCI (or populate J2`) and +VCXTRX and J1 jumper is placed between +5V0 and +5VRF.
  * USB microB (5V) alternative way to supply power for LimeFEA mPCIe board (make sure inserted mPCIe board supports 5V supply). In this case RF make sure J2 jumper is placed between +5VBUS and +VCXTRX and J1 jumper is placed between +5VBUS and +5VRF.
  * Header (3.3V or 5V) also may be used to power LimeFEA mPCIe board. Use only if USB or PCIe power is unavailable. It should only power PCIe mini expansion card but if RF front end is needed connect J2 jumper is between +5VBUS and +VCXTRX and place J1 jumper between +5VBUS and +5VRF. Keep in mind that RF front end requires 5V power input.
