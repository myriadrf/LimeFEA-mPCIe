RF Front End (Full)
###################################

LimeFEA mPCIe Full variant features RF front end with power amplifiers, low noise amplifiers and SPDT switches as shown in figure 4.

.. figure:: /images/LimeFEA-mPCIe_v1.0_RFFE.svg
  :width: 600

  Figure 4: LimeFEA mPCIe v1.0 Full RF path block diagram

A single control signal (TDD_GPIO3_N) is used to control all RF switches simultaneously for both A and B channels to change between TDD and FDD modes as shown in table 4.

.. list-table:: Table 4. RF path truth table
   :header-rows: 1

   * - Control signal (TDD_GPIO3_N)
     - TRX A/B Connected to
     - LNAin A/B Connected to
   * - Low
     - TXin A/B
     - LNAout A/B
   * - High
     - LNAout A/B
     - NC

RF path contains U.FL connectors (X13A/B, X14A/B) used for internal connections (for example to connect to LimeSDR XTRX) and (X15A/B, X16A/B) connecting antennas. 

Signal frequency range of TX and RX paths are listed in table 5.

.. list-table:: Table 5. RF path signal fequency range
   :header-rows: 1

   * - Direction
     - Frequency range
   * - TX
     - 100 MHz - 6 GHz
   * - RX
     - 100 MHz - 4 GHz

More detailed RF path component parameters are given in table 6.

.. table:: Table 6. RFFE components

  +---------------+--------------+--------------------+--------------+----------------------+------------+
  | **Component** | **Function** | **Frequency, MHz** | **Gain, dB** | **Output P1dB, dBm** | **NF, dB** |
  |               |              |                    |              |                      |            |
  +---------------+--------------+--------------------+--------------+----------------------+------------+
  | TQP3M9018     | TX amplifier | 900                | 22.4         | 21.4                 | 1.1        |
  |               |              +--------------------+--------------+----------------------+------------+
  |               |              | 1900               | 20.5         | 21                   | 1.1        |
  |               |              +--------------------+--------------+----------------------+------------+
  |               |              | 4000               | 17           | 19.2                 | 2.5        |
  +---------------+--------------+--------------------+--------------+----------------------+------------+
  | SPF5043Z      | RX amplifier | 900                | 18.2         | 22.6                 | 0.8        |
  |               |              +--------------------+--------------+----------------------+------------+
  |               |              | 1900               | 12.9         | 22.7                 | 0.8        |
  |               |              +--------------------+--------------+----------------------+------------+
  |               |              | 3800               | 7            | 22.8                 | 1.5        |
  +---------------+--------------+--------------------+--------------+----------------------+------------+
  | SKY13286      | RF switch    | 1000               | -0.7         |                      |            |
  |               |              +--------------------+--------------+----------------------+------------+
  |               |              | 2000               | -0.8         | 30                   |            |
  |               |              +--------------------+--------------+----------------------+------------+
  |               |              | 6000               | -1.6         |                      |            |
  +---------------+--------------+--------------------+--------------+----------------------+------------+