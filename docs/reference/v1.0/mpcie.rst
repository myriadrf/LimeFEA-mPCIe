Mini PCIe Socket
################

LimeFEA mPCIe board features mini PCIe specification compatible socket. Mini PCIe specification defines only 1 PCIe lane, but LimeFEA mPCIe features 2 PCIe lanes. Also mPCIe socket provides synchronization signals for LimeSDR XTRX board. More detailed information is listed in table 3.

.. list-table:: Table 3. mPCIe connector (X5) pinout
   :header-rows: 1
   :stub-columns: 1

   * - Pin
     - Mini PCIe Specification 
       
       Reference
     - LimeFEA mPCIe Schematic 
       
       Signal Name
     - LimeSDR XTRX Schematic 
       
       Signal Name
     - LimeSDR XTRX Description
   * - 1
     - Wake#
     - NC/RPI_PCIE_DET_nWAKE
     - NC
     - Not connected
   * - 2
     - 3.3 Vaux
     - VCC3P3
     - VCC3P3_MPCIE
     - Main power input
   * - 3
     - COEX1
     - PCIE_COEX1
     - 1PPSI_GPIO1(1N)
     - 1PPS input / GPIO1N
   * - 4
     - GND
     - GND
     - GND
     - Ground
   * - 5
     - COEX2
     - PCIE_COEX2
     - 1PPSO_GPIO2(1P)
     - 1PPS output / GPIO1P
   * - 6
     - GND
     - VCC1P5
     - NC
     - Not connected
   * - 7
     - CLKREQ#
     - RPI_PCIE_CLK_nREQ
     - CLK_REQUEST#
     - Tied to GND through 330 Ω resistor
   * - 8
     - UIM PWR
     - UIM_PWR
     - UIM_VCC
     - User Identity Module interface power 1.8 V or 3 V
   * - 9
     - GND
     - GND
     - GND
     - Ground
   * - 10
     - UIM_DATA
     - UIM_DATA
     - UIM_DIO
     - User Identity Module interface data 1.8 V or 3 V
   * - 11
     - REFCLK-
     - RPI_PCIE_CLK_N
     - PCI_REF_CLK_N
     - PCI Express reference clock differential pair negative signal
   * - 12
     - UIM_CLK
     - UIM_CLK
     - UIM_CLK
     - User Identity Module interface clock 1.8 V or 3 V
   * - 13
     - REFCLK+
     - RPI_PCIE_CLK_P
     - PCI_REF_CLK_P
     - PCI Express reference clock differential pair positive signal
   * - 14
     - UIM_RESET
     - UIM_RESET
     - UIM_RST
     - User Identity Module interface reset 1.8 V or 3 V
   * - 15
     - GND
     - GND
     - GND
     - Ground
   * - 16
     - UIM_VPP
     - UIM_VPP
     - NC
     - Not connected
   * - 17
     - Reserved
     - PCIE_UIM8
     - TDD_GPIO3_N
     - TDD TX Enable output or GPIO3N / GPIO4, CMOS 3.3 V
   * - 18
     - GND
     - GND
     - GND
     - Ground
   * - 19
     - Reserved
     - PCIE_UIMC4
     - CLK_IN
     - External clock input 3.3 V
   * - 20
     - W_DISABLE#
     - NC
     - TDD_GPIO3_P
     - GPIO3P or GPIO3 (pair of TDD TX Enable), CMOS 3.3 V
   * - 21
     - GND
     - GND
     - GND
     - Ground
   * - 22
     - PERST#
     - RPI_PCIE_nRST
     - PCIE_PERST#
     - PCI Express interface reset
   * - 23
     - PERn0
     - RPI_PCIE_RX_N
     - PCI_TX0_N
     - PCI Express interface output differential pair negative signal
   * - 24
     - 3.3Vaux
     - VCC3P3
     - NC
     - Not connected
   * - 25
     - PERp0
     - RPI_PCIE_RX_P
     - PCI_TX0_P
     - PCI Express interface output differential pair positive signal
   * - 26
     - GND
     - GND
     - GND
     - Ground
   * - 27
     - GND
     - GND
     - GND
     - Ground
   * - 28
     - 1.5Volt
     - VCC1P5
     - NC
     - Not connected
   * - 29
     - GND
     - GND
     - GND
     - Ground
   * - 30
     - SMB CLK
     - PCIE_SMB_CLK
     - SMB_CLK
     - Clock output (CLK_OUT)
   * - 31
     - PETn0
     - PCIE_PET0_N
     - PCI_RX0_N
     - PCI Express interface input differential pair negative signal
   * - 32
     - SMB Data
     - PCIE_SMB_DATA
     - SMB_DATA
     - GPIO8
   * - 33
     - PETp0
     - PCIE_PET0_P
     - PCI_RX0_P
     - PCI Express interface input differential pair positive signal
   * - 34
     - GND
     - GND
     - GND
     - Ground
   * - 35
     - GND
     - GND
     - GND
     - Ground
   * - 36
     - USB_D-
     - PCIE_USB_N
     - USB_D_N
     - USB 2.0 data differential pair negative signal
   * - 37
     - GND
     - GND
     - GND
     - Ground
   * - 38
     - USB_D+
     - PCIE_USB_P
     - USB_D_P
     - USB 2.0 data differential pair positive signal
   * - 39
     - 3.3Vaux
     - VCC3P3
     - PCI_TX1_N
     - PCI Express interface output differential pair negative signal
   * - 40
     - GND
     - GND
     - GND
     - Ground
   * - 41
     - 3.3Vaux
     - VCC3P3
     - PCI_TX1_P
     - PCI Express interface output differential pair positive signal
   * - 42
     - LED_WWAN#
     - PCIE_LED_WWAN
     - LED_WWAN#_GPIO5
     - Output for LED WWAN (negative) or GPIO5, 3.3 V
   * - 43
     - GND
     - GND
     - GND
     - Jumper to GND, connected by default
   * - 44
     - LED_WLAN#
     - PCIE_LED_WLAN
     - LED_WLAN#_GPIO6
     - Jumper to GND, connected by default
   * - 45
     - Reserved
     - NC
     - PCIE_RESERVED
     - Connected to FPGA (V7)
   * - 46
     - LED_WPAN#
     - PCIE_LED_WPAN
     - LED_WPAN#_GPIO7
     - Output for LED WPAN (negative) or GPIO7, 3.3 V
   * - 47
     - Reserved
     - NC
     - PCI_RX1_N
     - PCI Express interface input differential pair negative signal
   * - 48
     - 1.5Volt
     - VCC1P5
     - NC
     - Not connected
   * - 49
     - Reserved
     - NC
     - PCI_RX1_P
     - PCI Express interface input differential pair positive signal
   * - 50
     - GND
     - GND
     - GND
     - Ground
   * - 51
     - Reserved
     - NC
     - PCIE_W_DISABLE2#
     - Connected to FPGA (W3)
   * - 52
     - 3.3Vaux
     - VCC3P3
     - VCC3P3_MPCIE
     - Main power input 3.3 V (VCC3P3_MPCIE)