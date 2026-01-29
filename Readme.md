# MVP Scope — Wind Flow Visualization Simulator

## 1. Car Model Loading
- Include one built-in static mesh (e.g., a simple car model).
- Allow camera rotation, zoom, and orbit controls.
- No custom model uploads.

## 2. Environment Controls
- UI slider for wind speed (0–200 km/h).
- UI slider or buttons for wind direction (0–360 degrees or preset directions).
- Reset button for default values.

## 3. Basic Aerodynamic Calculations
Use simplified drag force formula:

```
F_drag = 0.5 * rho * v^2 * Cd * A
```

Fixed parameters for MVP:
- rho = 1.225
- Cd = 0.30
- A = 2.2 m²

Display outputs:
- Drag Force (N)
- Dynamic Pressure
- Wind speed and direction

## 4. Airflow Visualization (Simple Approximation)
Option A: Particle streams  
- Emit particles from wind direction.  
- Slightly deflect particles around car using simple distance-based forces.

Option B: Debug lines  
- Spawn several moving lines or arrows toward the car.  
- Bend trajectory around the vehicle when close.

Either method is acceptable for MVP.

## 5. UI Metrics Panel
- Show wind speed.
- Show wind direction.
- Show drag force.
- Show dynamic pressure.

## Out of Scope (Not for MVP)
- Real CFD simulation or turbulence.
- Pressure maps or heatmaps.
- Custom 3D model uploads.
- Mesh subdivision or voxelization.
- Vehicle movement or full driving simulation.
- Multi-vehicle scenarios.
