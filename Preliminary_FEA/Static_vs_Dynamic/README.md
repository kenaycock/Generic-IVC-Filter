# Static vs Dynamic

*Demonstration of a case where the static solver diverges while the dynamic solver converges:*

**Boundary conditions during Valsalva:**
  - Filter hub: **translation constrained in 'y' and 'z', but not in the axial direction, 'x'.**
  - Plate: fixed displacement representing reduction in the minor diameter of the IVC during the Valsalva maneuver
  - Distal end of filter strut: unconstrained, but there is a contact interaction between the strut surface and the plate that represents the vein wall.
    - Tangential friction is set relatively high (0.2); distal end of filter strut *"rocks"* along plate surface
  - **Files:**
    1. ...Static_BCs1.inp (diverges during step 3, 'valsalva1') 
    2. ...Dynamic_BCs1.inp 


<br><br>
*If the boundary conditions are tweaked slightly, the static simulation converges:*

**Boundary conditions during Valsalva:**
  - Filter hub: **translation constrained in 'x', 'y' and 'z' directions.**
  - Plate: fixed displacement representing reduction in the minor diameter of the IVC during the Valsalva maneuver
  - Distal end of filter strut: unconstrained, but there is a contact interaction (including tangential friction) between the strut surface and the plate that represents the vein wall.
    - Tangential friction is set relatively low (0.02); distal end of filter strut *slides* along plate surface
  - **Files:**
    1. ...Static_BCs2.inp
    
<br><br>
CORRESPONDENCE
--------------
**Feedback from Karthik:**
  - Static solver will not converge when there is unconstrained rigid body motion. Adjust boundary conditions accordingly in the future, or use Dynamic/Implicit and ensure that kinetic energy is a small (\<\<1%) fraction of the total internal energy.
