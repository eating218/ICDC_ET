== area.log ==
****************************************
Report : area
Design : LCD_CTRL
Version: Q-2019.12
Date   : Sun Aug  3 20:15:17 2025
****************************************

Library(s) Used:

    slow (File: /usr/cad/LIB/CBDK_TSMC90G_Arm_v1.1/CIC/SynopsysDC/db/slow.db)

Number of ports:                          163
Number of nets:                         13060
Number of cells:                        12900
Number of combinational cells:          12333
Number of sequential cells:               557
Number of macros/black boxes:               0
Number of buf/inv:                       1902
Number of references:                      64

Combinational area:              52503.697185
Buf/Inv area:                     5684.313749
Noncombinational area:            8647.833620
Macro/Black Box area:                0.000000
Net Interconnect area:      undefined  (No wire load specified)

Total cell area:                 61151.530805
Total area:                 undefined

== timing.log ==
****************************************
Report : timing
        -path full
        -delay max
        -max_paths 1
Design : LCD_CTRL
Version: Q-2019.12
Date   : Sun Aug  3 20:15:17 2025
****************************************

Operating Conditions: slow   Library: slow
Wire Load Model Mode: top

  Startpoint: cmd[2] (input port clocked by clk)
  Endpoint: system_array_reg[7][7][3]
            (rising edge-triggered flip-flop clocked by clk)
  Path Group: clk
  Path Type: max

  Point                                                   Incr       Path
  --------------------------------------------------------------------------
  clock clk (rise edge)                                   0.00       0.00
  clock network delay (ideal)                             0.50       0.50
  input external delay                                    5.00       5.50 f
  cmd[2] (in)                                             0.01       5.51 f
  U6556/Y (INVX2)                                         0.04       5.55 r
  U6555/Y (NOR2X2)                                        0.03       5.58 f
  U5269/Y (NOR3BX1)                                       0.10       5.68 f
  U4737/Y (NOR2BX1)                                       0.14       5.83 f
  U4242/Y (AOI22XL)                                       0.08       5.91 r
  U4240/Y (OAI211XL)                                      0.13       6.04 f
  U3743/Y (NOR2BX1)                                       0.14       6.18 f
  U4223/Y (AOI221XL)                                      0.11       6.29 r
  U4221/Y (OAI211XL)                                      0.60       6.89 f
  U4220/Y (INVX2)                                         0.11       7.00 r
  U3750/Y (INVX2)                                         0.17       7.17 f
  U5160/Y (AOI222XL)                                      0.21       7.38 r
  U5158/Y (OAI211XL)                                      0.13       7.51 f
  system_array_reg[7][7][3]/D (DFFRQX2)                   0.00       7.51 f
  data arrival time                                                  7.51

  clock clk (rise edge)                                  10.00      10.00
  clock network delay (ideal)                             0.50      10.50
  clock uncertainty                                      -0.10      10.40
  system_array_reg[7][7][3]/CK (DFFRQX2)                  0.00      10.40 r
  library setup time                                     -0.05      10.35
  data required time                                                10.35
  --------------------------------------------------------------------------
  data required time                                                10.35
  data arrival time                                                 -7.51
  --------------------------------------------------------------------------
  slack (MET)                                                        2.84
