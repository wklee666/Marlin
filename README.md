New/Changed parameters in Configuration.h :

* DELTA_DIAGONAL_ROD  ->  DEFAULT_DELTA_DIAGONAL_ROD  - set default value only, can be changed by m666 Dxxx for which xxx is the new Diagonal Rod value
* DELTA_RADIUS        ->  DEFAULT_DELTA_RADIUS        - set default value only, can be changed by m666 Rxxx for which xxx is the new Radius value
* Tower and Tower Radius Adjustment (If you know it):
   *  Tower distance Adjust
      - DELTA_TOWER1_ADJ  0
      - DELTA_TOWER2_ADJ  0
      - DELTA_TOWER3_ADJ  0
   *  Tower Radius Adjust
      - DELTA_TOWER1_RAD_ADJ  0
      - DELTA_TOWER2_RAD_ADJ  0
      - DELTA_TOWER3_RAD_ADJ  0
* Z_RAISE_AFTER_PROBING 50    - How much the extruder will be raised after the last probing point.
* DEFAULT_XYZTOWER_PROBE_POS  - XYZ Probe Position (base on calculated value, you may ignore it if no problem)
* REPEAT_PROBE_PRECISION	    - precision of the repeated probe for one point

New/Modified GCODE :

* G30   - Probe 1 point at specified xy location, e.g. G30 X-45 Y40
* G31   - Auto calibration XYZ Enstop, parameter A for max number of run times, default 1, e.g. G31 A10 will run max 10 times
* G32   - Probe xyz and center, view only
  
* M666  - Added D to change DIAGONAL_ROD and R to change Radius