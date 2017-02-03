# Rev1.1

**Rev1 filter revised for manufacturability**

REVISIONS
---------
- [x] Account for
    1. laser beam cutting width (kerf) and
    2. material removal related to surface finishing (see *Open Stent* manuscript from C. Bonsignore for details)
- [x] Change the tubing from TSE0800X0525GS to TSE0800X0515GS to increase the wall thickness and compensate for material removed during surface finishing
    * same OD, new ID (1.3081mm here vs. 1.3335mm in Rev1; see https://shop.confluentmedical.com/collections/tube)
- [x] Add a flat configuration for the laser toolpath
- [x] Improve the drawing sheets
- [x] Create 2D "dxf" file for the laser toolpath (scale is 1:1)

NOTES
-----
* The following values were assumed based on those given in the *Open Stent* manuscript:
    * Laser kerf: 0.025mm
    * Material removal during finishing
        * width: 0.036mm (i.e., 0.018mm from each side)
        * thickness: 0.059mm (from *inside* surface to remove draw lines)
* ^ Are these values appropriate for this size of tubing and the material processing that we plan? I believe we decided on electropolishing.

CORRESPONDENCE
--------------
See https://github.com/kenaycock/Generic-IVC-Filter/issues/2
