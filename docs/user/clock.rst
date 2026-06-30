Reference Clock and 1PPS Connectors (only for full variant)
###########################################################

LimeFEA mPCIe board offers four :external+sdrxtrx:ref:`LimeSDR XTRX <index:introduction>` compatible reference clock and 1PPS U.FL connectors.  

.. figure:: /images/LimeFEA-mPCIe_v1.0_clkcon.png
  :width: 600
  
  Figure 4: LimeFEA mPCIe reference clock and 1PPS connectors

.. _ref-clk-table:

.. list-table:: Table 2. reference clock and 1PPS connectors
   :header-rows: 1

   * - Connector id
     - mPCIe pin
     - :external+sdrxtrx:ref:`LimeSDR XTRX <index:introduction>` description
   * - X3
     - 3
     - 1PPS input
   * - X4
     - 5
     - 1PPS output
   * - X11
     - 30
     - Clock output (CLK_OUT)
   * - X12
     - 19
     - External clock input 3.3 V


.. warning::
     Before using the reference clock and 1PPS  connectors, verify the pinout of the installed Mini PCIe device to ensure signal compatibility and prevent incorrect signal connections.


