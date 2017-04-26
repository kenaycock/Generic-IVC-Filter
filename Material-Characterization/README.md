# Material Characterization


UMAT material constants:

| Parameter | Value | 
|:-------------:|:-------------:| 
| E<sub>a</sub> | 59,000 MPa |
| 𝜈<sub>a</sub> | 0.33 |
| E<sub>m</sub> | 24,750 MPa |
| 𝜈<sub>m</sub> | 0.33 | 
| ε<sup>L</sup> | 0.042 |
| 𝛿σ/𝛿T<sub>L</sub> | 4.77 MPa / °C |
| σ<sup>S</sup><sub>L</sub> | 395 MPa |
| σ<sup>E</sup><sub>L</sub> | 435 MPa |
| T<sub>0</sub> | 37 °C |
| 𝛿σ/𝛿T<sub>U</sub> | 9.00 MPa / °C |
| σ<sup>S</sup><sub>U</sub> | 165 MPa |
| σ<sup>E</sup><sub>U</sub> | 145 MPa |
| σ<sup>S</sup><sub>cL</sub> | 395 MPa |
| ε<sup>L</sup><sub>V</sub> | 0.042 | 
| N<sub>A</sub> | 0 |
| N<sub>P</sub> | 3 |
| σ<sup>P</sup><sub>1</sub> | 1205 MPa |
| ε<sup>P</sup><sub>1</sub> | 0.090 |
| σ<sup>P</sup><sub>2</sub> | 1350 MPa |
| ε<sup>P</sup><sub>2</sub> | 0.100 |
| σ<sup>P</sup><sub>3</sub> | 1450 MPa | 
| ε<sup>P</sup><sub>3</sub> | 0.120 |

Plot of experimental data and ABAQUS UMAT with above constants:
![stress-strain_plot_37C_low_strain](https://github.com/kenaycock/Generic-IVC-Filter/blob/master/Material-Characterization/Material_Characterization_Data_Plots.png?raw=true)

The nitinol UMAT verification was performed using a single C3D8R element (one integration point). The logarithmic strain and the Cauchy stress were extracted from the ODB simulations results file.
