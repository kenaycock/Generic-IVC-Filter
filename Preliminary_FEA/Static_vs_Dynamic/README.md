# Static vs Dynamic

*Demonstration of a case where the static solver diverges while the dynamic solver converges:*

**Boundary conditions during Valsalva:**
  - Hub: **translation constrained in 'y' and 'z', but not in the axial direction, 'x'.**
  - Plate: fixed displacement representing reduction in the minor diameter of the IVC during the Valsalva maneuver
  - Distal end of filter strut: unconstrained, but there is a contact interaction between the strut surface and the plate that represents the vein wall.
    - Tangential friction is set relatively high (0.2)
  - **Files:**
    1. ...static_BCs1.inp (diverges during step 3) 
    2. ...dynamic_BCs1.inp 


<br><br>
*If the boundary conditions are tweaked slightly, both the static and the dynamic simulations converge:*

**Boundary conditions during Valsalva:**
  - Hub: **translation constrained in 'x', 'y' and 'z' directions.**
  - Plate: fixed displacement representing reduction in the minor diameter of the IVC during the Valsalva maneuver
  - Distal end of filter strut: unconstrained, but there is a contact interaction (including tangential friction) between the strut surface and the plate that represents the vein wall.
    - Tangential friction is set relatively low (0.02)
  - **Files:**
    1. ...static_BCs2.inp (diverges during step 3) 
    2. ...dynamic_BCs2.inp 
