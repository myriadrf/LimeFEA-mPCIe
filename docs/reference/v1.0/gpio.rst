GPIO Connector (unpopulated)
############################

Some mPCIe connector (X5) pins are connected to 2.54 mm pin header. By default it is not populated. GPIO header pinuot signals are not defined in specification and only used by LimeSDR XTRX board. GPIO header pins and additional information is given in table 7.

.. list-table:: Table 7. GPIO header pinout
   :header-rows: 1
   :stub-columns: 1

   * - Connector pin
     - Schematic signal name
     - mPCIe pin
     - I/O standard
     - Comment
   * - 1
     - GND
     - 
     - 
     - Ground (0V)
   * - 2
     - GPIO8
     - 32
     - 3.3V
     - General purpose
   * - 3
     - GPIO3P
     - 20
     - 3.3V
     - General purpose
   * - 4
     - GPIO3N
     - 17
     - 3.3V
     - TDD control