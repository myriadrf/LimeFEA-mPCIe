JTAG
####

LimeFEA mPCIe board has JTAG 2.54 mm pitch header to spring connector adapter that is designed to be used with LimeSDR XTRX. 
Since JTAG programmer can’t be connected directly to the LimeSDR XTRX board while it is sloted into mPCIe.
So JTAG header (X8) can be used to connect LimeSD XTRXT to JTAG programmer. More detailed information about JTAG header and its connection to spring connector (X10) is given in table 8.

.. list-table:: Table 8. JTAG Header and Spring Connector pinouts
   :header-rows: 1

   * - Schematic signal name
     - JTAG header (X8) pin
     - JTAG spring connector (X10) pin
     - Comment
   * - TMS
     - 1
     - 3
     - JTAG select
   * - TDI
     - 2
     - 2
     - JTAG data in
   * - TDO
     - 3
     - 1
     - JTAG data out
   * - TCK
     - 4
     - 5
     - JTAG clock
   * - GND
     - 5
     - 6
     - Ground
   * - +VIOXTRX
     - 6
     - 4
     - Power