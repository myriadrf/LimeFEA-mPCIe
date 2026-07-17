PCIe x4 Edge Connector
######################

LimeFEA mPCIe board is a low-profile PCIe expansion card designed to fit into x4 (or bigger) slots (2 PCIe lanes are used). PCIe edge connector pinuot, schematic signal names and descriptions are listed in table 2.

.. list-table:: Table 2.  PCIe x4 edge connector (X2) pinout
   :header-rows: 1
   :stub-columns: 1

   * - Pin
     - PCIe Specification Reference
     - Schematic Signal Name
     - PCIe Specification Description
   * - B1
     - +12V
     - +12VIN
     - Power (12V)
   * - A1
     - PRSNT#1
     - SIZEX4
     - Hot plug detect
   * - B2
     - +12V
     - +12VIN
     - Power (12V)
   * - A2
     - +12V
     - +12VIN
     - Power (12V)
   * - B3
     - +12V
     - +12VIN
     - Power (12V)
   * - A3
     - +12V
     - +12VIN
     - Power (12V)
   * - B4
     - GND
     - GND
     - Ground (0V)
   * - A4
     - GND
     - GND
     - Ground (0V)
   * - B5
     - SMBCLK
     - NC
     - SMBus clock
   * - A5
     - JTAG-TCK
     - NC
     - TCK
   * - B6
     - SMBDAT
     - NC
     - SMBus data
   * - A6
     - JTAG-TDI
     - NC
     - TDI
   * - B7
     - GND
     - GND
     - Ground (0V)
   * - A7
     - JTAG-TDO
     - NC
     - TDO
   * - B8
     - +3.3V
     - +3,3VPCI
     - Power (3.3V)
   * - A8
     - JTAG-TMS
     - NC
     - TMS
   * - B9
     - JTAG-RST
     - NC
     - +TRST#
   * - A9
     - +3.3V
     - +3,3VPCI
     - Power (3.3V)
   * - B10
     - +3.3Vaux
     - NC
     - Power (3.3V)
   * - A10
     - +3.3V
     - +3,3VPCI
     - Power (3.3V)
   * - B11
     - Wake#
     - NC
     - Link reactivation
   * - A11
     - PWRGOOD
     - PCI_PERST#
     - Reset signal
   * - B12
     - Reserved
     - NC
     - No connection
   * - A12
     - GND
     - GND
     - Ground (0V)
   * - B13
     - GND
     - GND
     - Ground (0V)
   * - A13
     - REFCLK+
     - PCI_REF_CLK_P
     - Reference clock +
   * - B14
     - HSOp(TX0p)
     - PCI_RX0_P
     - Transmitter lane 0 +
   * - A14
     - REFCLK-
     - PCI_REF_CLK_N
     - Reference clock -
   * - B15
     - HSOn(TX0n)
     - PCI_RX0_N
     - Transmitter lane 0 -
   * - A15
     - GND
     - GND
     - Ground (0V)
   * - B16
     - GND
     - GND
     - Ground (0V)
   * - A16
     - HSIp(Rx0p)
     - PCI_TX0_P
     - Receiver lane 0 +
   * - B17
     - PRSNT#1 (x1)
     - NC
     - Hotplug detect
   * - A17
     - HSIn(Rx0n)
     - PCI_TX0_N
     - Receiver lane 0 -
   * - B18
     - GND
     - GND
     - Ground (0V)
   * - A18
     - GND
     - GND
     - Ground (0V)
   * - B19
     - HSOp(Tx1p)
     - PCI_RX1_P
     - Transmitter lane 1 +
   * - A19
     - Reserved
     - NC
     - No connection
   * - B20
     - HSOn(Tx1n)
     - PCI_RX1_N
     - Transmitter lane 1 -
   * - A20
     - GND
     - GND
     - Ground (0V)
   * - B21
     - GND
     - GND
     - Ground (0V)
   * - A21
     - HSIp(Rx1p)
     - PCI_TX1_P
     - Receiver lane 1 +
   * - B22
     - GND
     - GND
     - Ground (0V)
   * - A22
     - HSIn(Rx1n)
     - PCI_TX1_N
     - Receiver lane 1 -
   * - B23
     - HSOp(Tx2p)
     - NC
     - Transmitter lane 2 +
   * - A23
     - GND
     - GND
     - Ground (0V)
   * - B24
     - HSOn(Tx2n)
     - NC
     - Transmitter lane 2 -
   * - A24
     - GND
     - GND
     - Ground (0V)
   * - B25
     - GND
     - GND
     - Ground (0V)
   * - A25
     - HSIp(Rx2p)
     - NC
     - Receiver lane 2 +
   * - B26
     - GND
     - GND
     - Ground (0V)
   * - A26
     - HSIn(Rx2n)
     - NC
     - Receiver lane 2 -
   * - B27
     - HSOp(Tx3p)
     - NC
     - Transmitter lane 3 +
   * - A27
     - GND
     - GND
     - Ground (0V)
   * - B28
     - HSOn(Tx3n)
     - NC
     - Transmitter lane 3 -
   * - A28
     - GND
     - GND
     - Ground (0V)
   * - B29
     - GND
     - GND
     - Ground (0V)
   * - A29
     - HSIp(Rx3p)
     - NC
     - Receiver lane 3 +
   * - B30
     - Reserved
     - NC
     - No connection
   * - A30
     - HSIn(Rx3n)
     - NC
     - Receiver lane 3 -
   * - B31
     - PRSNT#2 (x4)
     - SIZEX4
     - Hotplug detect
   * - A31
     - GND
     - GND
     - Ground (0V)
   * - B32
     - GND
     - GND
     - Ground (0V)
   * - A32
     - Reserved
     - NC
     - No connection