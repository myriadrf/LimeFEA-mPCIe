Hardware Setup
##############

Host Interface
**************

LimeFEA mPCIe provides PCIe x4 and USB Micro-B connectivity interfaces for Mini PCIe modules.

PCIe
====

LimeFEA mPCIe is designed for installation in a PCIe x4 or higher slot, providing an interface between the host system and the connected Mini PCIe device

The host must provide a PCIe Gen2 x1 or x2 interface, and supply power (3.3V) via the PCIe connector.

.. note::
   Both PCIe lanes can only be used by Mini PCIe devices that support 2x lane data transfer.

USB
===

USB Micro-B cable can be used to interface with an plugged in Mini PCIe device. 

The host system must provide a USB 2.0 interface and supply 5 V power through the USB Micro-B connector.

.. warning::
   Make sure installed Mini PCIe device supports 5V input power.
   
Cooling
*******

LimeFEA mPCIe features a 35 mm x 17 mm dimensions exposed copper pad near mPCIe connector (X5). 

Thermal gap filler can be applied on the exposed copper pad to help with mini PCIe expansion board heat disipation.

In case that :external+sdrxtrx:ref:`LimeSDR XTRX <index:introduction>` is used we recommend 30 mm x 17 mm thermal gap filler with a thickness of 0.5 mm. Place it starting from mPCIe connector side leaving copper near standoffs uncovered as shown in figure 6.

.. figure:: /images/LimeFEA-mPCIe_v1.0_XTRX_thermal_pad.png
  :width: 600

  Figure 2: Recommended thermal gap filler dimensions and placement for :external+sdrxtrx:ref:`LimeSDR XTRX <index:introduction>`

RF Connections (only for full variant)
**************************************

.. figure:: /images/LimeFEA-mPCIe_v1.0_rfcon.png
  :width: 600
  
  Figure 3: LimeFEA XTRX v1.3 board top with RF connector positions

.. list-table:: Table 1. RF Connectors
      :header-rows: 1      

      * - Connector
        - Type
        - Function
        - Frequency range
      * - X13A (Ch A), X13B (Ch B)
        - U.FL
        - TX input
        - 0.1–6 GHz
      * - X16A (Ch A), X16B (Ch B)
        - U.FL
        - RX input
        - 0.1–4 GHz
      * - X14A (Ch A), X14B (Ch B)
        - U.FL
        - RX output
        - 0.1–4 GHz
      * - X15A (Ch A), X15B (Ch B)
        - U.FL
        - TRX input/output
        - 0.1–4 GHz

.. warning::
   Care should be taken when connecting external RF signals to the RX inputs, to ensure that the maximum safe input power of +10 dBm is not exceeded, as this may cause permanent damage to the device.