Power Distribution
##################

LimeFEA mPCIe board power delivery network consists of different power rails with different regulators, voltages and filters. LimeFEA mPCIe board power distribution block diagram is presented in figure 6.

.. figure:: /images/LimeFEA-mPCIe_v1.0_power.svg
  :width: 600

  Figure 6: LimeFEA mPCIe v1.0 power distribution block diagram

Power Sources
=============

The LimeFEA mPCIe board supports multiple input power configurations to accommodate different use cases.

PCIe x4 Edge Connector
----------------------

The PCIe edge connector is the preferred power source for the LimeFEA mPCIe board. The host system must provide both 12V and 3.3V supply rails through the PCIe x4 connector.

Ensure that:

* J2 jumper is installed between +3.3VPCI (or populate J2′) and +VCXTRX to power mPCIe device.
* J1 jumper is installed between +5V0 and +5VRF to power the RF front end. (only for full version)

USB microB connector
--------------------

The USB connector can be used as an alternative power source for the LimeFEA mPCIe board when the preferred PCIe power rails are not available.

In this configuration, ensure that:

* J2 jumper is installed between +5VBUS and +VCXTRX to power mPCIe device.
* J1 jumper is installed between +5VBUS and +5VRF to power the RF front end. (only for full version)

.. warning::
  A 5V (USB) power supply is not part of the standard mPCIe power specification. Use a 5V USB power supply only if it is explicitly supported or approved by the device manufacturer. (e.g., LimeSDR XTRX does allow 5V power supply voltage)

Header
------
The power header (X17) can also be used to power the LimeFEA mPCIe board when neither PCIe nor USB power is available.

Configure the jumpers as follows:

* Install J2 jumper between +5VBUS and +VCXTRX to power mPCIe device.
* Install J1 jumper between +5VBUS and +5VRF to power the RF front end. (only for full version)

.. warning::
  The RF front end requires a 5 V supply, whereas mPCIe devices typically require 3.3 V. If both the RF front end and the mPCIe device are powered from the header, verify that the mPCIe device supports a 5 V input before applying power.

