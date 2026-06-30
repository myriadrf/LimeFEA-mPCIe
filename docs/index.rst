Introduction
############

.. toctree::
   :maxdepth: 3
   :hidden:
   
   Introduction <self>
   user/index
   reference/index
   developer

.. tabs::
    
  .. tab:: LimeFEA mPCIe Full

    .. figure:: images/LimeFEA-mPCIe_v1.0_3D_isofull.png
      :align: center

  .. tab:: LimeFEA mPCIe Lite

    .. figure:: images/LimeFEA-mPCIe_v1.0_3D_isolight.png
      :align: center

The LimeFEA mPCIe is a PCIe-to-mini PCIe adapter board designed to provide a flexible hardware platform for developing and deploying high-performance systems based on mini PCIe modules. The board provides a two-lane PCI Express interface and a mini PCIe socket compatible with the LimeSDR XTRX software-defined radio module, enabling integration of SDR capabilities into systems equipped with standard PCIe expansion slots.

The LimeFEA mPCIe is available in two variants: the LimeFEA mPCIe Lite and the LimeFEA mPCIe Full. The LimeFEA mPCIe Lite provides the essential PCIe-to-mini PCIe conversion functionality, allowing the connection and operation of compatible mini PCIe modules without additional RF circuitry. The LimeFEA mPCIe Full extends the platform capabilities by incorporating an integrated radio-frequency front end (RFFE), providing additional transmit and receive functionality through RF amplification, low-noise amplification, RF switching, and associated control circuitry.

In addition to RF functionality, the LimeFEA mPCIe Full variant provides interfaces for external synchronization signals, JTAG programming, USB connectivity, SIM card support, and multiple RF connections. These features make the board suitable for wireless communication research, SDR prototyping, and embedded RF system development.

Specifications
**************

RF
==

.. list-table:: 
   :header-rows: 1
   :stub-columns: 1

   * - Parameter
     - Value
     - Notes
   * - Configuration
     - MIMO (2T2R)
     - 2 Full-duplex channels
   * - Frequency Range
     - 100 MHz – 4 GHz
     - Continuous coverage
   * - Rx Gain
     - 12.9 dB
     - Depends on frequency
   * - Tx Gain
     - 20.5 dB
     - Depends on frequency 
   * - Max. Safe Rx Input Power
     - 10 dBm
     - Absolute maximum
   * - Max. Safe Tx Input Power
     - 10 dBm
     - Absolute maximum


Digital Interfaces
==================

* PCIe x4 to mini PCIe edge connector adapter with PCIe Gen 2 x2.
* USB Micro-B to mini PCIe connector adapter with USB 2.0.
* JTAG 2.54 mm pitch header to spring connector adapter for :external+sdrxtrx:ref:`LimeSDR XTRX <index:introduction>`.

.. note::
  Both PCIe lanes can only be used with devices such as :external+sdrxtrx:ref:`LimeSDR XTRX <index:introduction>` that support 2 lane data transfer.

Power Supply
============

.. list-table:: 
   :header-rows: 1
   :stub-columns: 1

   * - Parameter
     - Value
     - Notes
   * - Input Voltage (mPCIe)
     - 3.3 V DC
     - Via mPCIe connector
   * - Input Voltage (USB)
     - 5 V DC
     - Via Micro-B USB connector
   * - Maximum Power (mPCIe)
     - 3.3 W
     - mPCIe limit

.. warning::
   When using USB (5V) as power source make sure that mPCIe device supports 5V input power.

Environmental
=============

.. list-table:: 
   :header-rows: 1
   :stub-columns: 1

   * - Parameter
     - Value
     - Notes
   * - Operating Temperature
     - 0 °C to +75 °C
     - Commercial-grade
   * - Storage Temperature
     - -40 °C to +85 °C
     - N/A
   * - Operating Humidity
     - 10% to 90% RH  
     - Non-condensing

Mechanical
==========

Board size: 68.9mm x 100mm (Low-Profile PCIe expansion card).

Features
********

Connectors
==========

  * PCIe x4 card edge connector (2 PCIe lanes)
  * Mini PCIe (1.55 mm heigth) connector (2 PCIe lanes)
  * USB 2.0 microB
  * JTAG (2.54 mm pitch) header that is connected to a spring connector (for LimeSDR XTRX)
  * Nano-SIM socket
  * Coaxial RF (12x U.FL female) connectors for RF front end and synchronization signals 

RF Front End
============

  * LNAs, PAs, RF switches, power and mode control (TDD and FDD)

General user inputs/outputs:
============================

  * 3x general purpose LEDs (PCIe indication by default)
  * 3x general purpose I/Os (unpopulated)
  * Power source selection for mini PCIe card and RFFE (2.54 mm pitch headers)



Purchasing
**********

Please see the  `Crowd Supply Website`_ for purchasing options.

Regulatory
**********

RoHS
====

This product is RoHS compliant and does not contain hazardous substances as defined by Directive 2011/65/EU.

WEEE
====

This product must be disposed of properly according to local regulations. Do not dispose of with general household waste.

RF Transmission Notice
======================

.. warning::
   Operating RF transmitting equipment may require appropriate licensing. Users are responsible for ensuring compliance with local regulations. Unauthorised transmission may result in legal penalties.


.. _Crowd Supply Website: https://www.crowdsupply.com/lime-micro/limefea-mpcie-carrier-board
