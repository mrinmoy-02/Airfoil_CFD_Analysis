Airfoil Aerodynamics Analysis Using ANSYS Fluent

This project presents a Computational Fluid Dynamics (CFD) analysis of an airfoil using ANSYS Fluent, a leading fluid simulation software. The aim of this project is to simulate and understand the aerodynamic performance of an airfoil, particularly focusing on the forces of lift and drag under specified conditions. This analysis provides insights that can be crucial for optimizing the airfoil design used in aircraft and other aerodynamic applications.

Project Overview
- Software: The analysis was conducted using ANSYS Fluent v24.1.0, a state-of-the-art CFD tool capable of simulating complex fluid phenomena. The software supports 3D simulations with double precision, and this project employs the steady-state model with SST k-omega turbulence to capture the airfoil's aerodynamic behavior.
- Objective: The primary goal is to compute key aerodynamic metrics, such as drag coefficient, drag force, and lift force, while also visualizing the airflow around the airfoil using contour plots.

Mesh and Geometry Setup
- Airfoil Geometry: The airfoil was modeled within a fluid domain, ensuring the proper representation of the aerodynamic shape.
- Mesh Quality: A fine mesh was created with 969,528 cells, 2,096,388 faces, and 261,154 nodes, ensuring that the airfoil's surface and the surrounding airflow are accurately represented. The minimum orthogonal quality of the mesh was 0.1056, with a maximum aspect ratio of 43.56, which guarantees a good balance between computational cost and accuracy.

Simulation Setup
- Boundary Conditions: 
  - Inlet: Velocity was set at 48 m/s, directed normal to the boundary, representing typical airspeed conditions.
  - Outlet: The gauge pressure was set at 0 Pa, ensuring proper flow conditions at the exit.
  - Wall: The no-slip condition was applied to the airfoil surface to model the aerodynamic drag accurately.
- Turbulence: The SST k-omega turbulence model was employed to simulate high-accuracy turbulence, with a turbulent intensity of 5% and a viscosity ratio of 10. These parameters ensure that the flow separation and aerodynamic forces are realistically predicted.

Key Metrics and Results
1. Coefficient of Drag (Cd): The drag coefficient was calculated as 1.676, which represents the resistance experienced by the airfoil as it moves through the air. Reducing this value is crucial in aerodynamic optimization.
2. Drag Force: The total drag force acting on the airfoil was computed as 1.02673 N, which quantifies the air resistance faced by the airfoil.
3. Lift Force: The lift force, a critical measure for any airfoil, was calculated at 6.708154 N. This value indicates the airfoil's ability to generate lift, crucial for flight stability and performance.
4. Solver Convergence: The simulation achieved convergence after 507 iterations, indicating that the solution was stable and accurate.

Post-Processing and Visualization
- Contour Plots: The post-processing results include pressure and velocity contours, which provide a visual representation of how air flows over the airfoil's surface. These plots help in identifying areas of high and low pressure, flow separation, and regions that contribute to lift and drag.

Conclusion
The CFD analysis of this airfoil using ANSYS Fluent provides a detailed understanding of the airfoil’s aerodynamic properties. The key findings, such as drag and lift forces, combined with visual data from contour plots, offer valuable insights for optimizing airfoil designs in aviation and other industries that rely on efficient airflow management.
