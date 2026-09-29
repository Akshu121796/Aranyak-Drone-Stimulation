# 🚁 DroneEye — 3D Disaster Response Simulation

DroneEye is a realistic 3D drone-based disaster-response simulation designed to demonstrate autonomous aerial monitoring, disaster detection, and search-and-rescue workflows.

The simulation provides an interactive environment where a drone can navigate through different disaster scenarios, identify hazards or survivors, and display real-time visual alerts.

---

## 🌍 Key Features

### 🚁 Drone Navigation

- Smooth 3D drone movement
- Autonomous navigation during mission scenarios
- Real-time flight telemetry
- Multiple camera perspectives
- Interactive environment exploration

---

### 🔥 Fire Detection

The simulation includes an active fire-disaster scenario.

When the drone approaches the fire region:

- Fire becomes visibly active with flames, smoke and embers
- The fire region is detected
- A visual bounding box highlights the detected area
- `FIRE DETECTED` appears in the HUD
- Detection confidence is displayed

This demonstrates how a drone can identify and monitor a fire-affected region.

---

### 🌊 Flood Detection

A dedicated flooded region represents a flood-disaster scenario.

When the drone approaches the affected region:

- The flooded area is detected
- A visual detection boundary highlights the affected region
- `FLOOD DETECTED` appears in the HUD
- Detection information is displayed in real time

This demonstrates aerial monitoring of flood-affected areas.

---

### ⛰️ Landslide & Survivor Detection

The simulation contains a landslide/debris region with visible survivors.

When the drone approaches the search area:

- Human survivors are detected
- Bounding boxes identify detected people
- `SURVIVOR DETECTED` appears in the HUD
- Detection confidence is displayed

This demonstrates how UAVs can support search-and-rescue operations after a landslide.

---

# 🎮 Controls

| Key | Function |
|-----|----------|
| `W` | Move Forward |
| `S` | Move Backward |
| `A` | Move Left |
| `D` | Move Right |
| `Q` | Move Down |
| `E` | Move Up |
| `V` | Change Camera Mode |
| `T` | Toggle Thermal View |
| `F` | Toggle Fog |
| `Space` | Toggle Autonomous Patrol |
| `H` | Show / Hide Help |

---

## 📷 Camera Modes

DroneEye provides multiple camera perspectives for monitoring the disaster environment.

### Cinematic

A smooth third-person camera that follows the drone and provides a cinematic view of the mission.

### FPV

A first-person perspective from the drone, useful for close-range inspection.

### Free Orbit

Allows the user to interactively rotate and inspect the environment around the drone.

### Overhead

Provides a bird's-eye tactical view of the disaster area.

Press `V` to switch between camera modes.

---

# 🌡️ Thermal View

Press `T` to toggle thermal visualization.

Thermal mode provides an alternative visualization layer for disaster-response scenarios and can assist with identifying areas of interest under reduced-visibility conditions.

---

# 🌫️ Fog

Press `F` to toggle environmental fog.

Fog can be used to simulate reduced visibility during disaster-response missions and demonstrate how the drone operates under changing environmental conditions.

---

# 🛰️ Mission & Telemetry

The HUD provides real-time information about the drone and current mission.

### Flight Telemetry

- Altitude
- Speed
- Battery
- Distance
- Heading
- Pitch
- Roll

### Mission Information

- Current mission status
- Active detection alerts
- Risk information
- Disaster detection status

### Tactical Map

The simulation also includes a tactical minimap showing the drone's position and important areas within the environment.

---

# 🔄 Disaster Response Workflow

The simulation follows a simplified autonomous disaster-response workflow:

```text
Drone Deployment
       ↓
Environment Monitoring
       ↓
Disaster Scenario
       ↓
Autonomous Navigation
       ↓
Hazard / Human Detection
       ↓
Bounding Box + Detection Alert
       ↓
Telemetry & Mission Update
🚨 Demonstrated Scenarios
🌊 Flood Scenario
Drone Deployment
       ↓
Flooded Region
       ↓
Drone Approaches Area
       ↓
Flood Detection
       ↓
FLOOD DETECTED
       ↓
HUD + Detection Boundary
🔥 Fire Scenario
Fire Outbreak
       ↓
Drone Detects Mission Target
       ↓
Autonomous Navigation
       ↓
Fire Region
       ↓
FIRE DETECTED
       ↓
Bounding Box + HUD Alert
⛰️ Landslide & Survivor Scenario
Landslide / Debris Region
       ↓
Search Area
       ↓
Drone Approaches
       ↓
Human Detection
       ↓
SURVIVOR DETECTED
       ↓
Human Bounding Box + HUD Alert
🛠️ Technology Stack
Three.js — 3D rendering and simulation
JavaScript — simulation logic and interactions
HTML5 / CSS3 — interface and HUD
WebGL — browser-based 3D rendering
Procedural 3D Environment — terrain, vegetation, disaster zones and environmental effects

🎯 Purpose

DroneEye demonstrates how autonomous UAV systems can support disaster-response operations through:

Navigation + Environmental Monitoring + Hazard Detection + Human Detection + Real-Time Visualization

The simulation provides a visual proof-of-concept for aerial disaster assessment and search-and-rescue workflows.

📁 Project Structure
drone-disaster-simulation/
│
├── drone_simulation.html
└── README.md

🚀 Running Locally

Because the simulation uses browser-based 3D resources, it is recommended to run it through a local HTTP server instead of opening the HTML file directly.

1. Open the project directory
cd animation
2. Start a local server
python -m http.server 8000
3. Open in your browser
http://localhost:8000/drone_simulation.html

🔮 Future Extensions

Possible future improvements include:

Real computer-vision detection models
Live drone telemetry
GPS-based disaster mapping
Real-time sensor integration
Edge AI inference
Disaster-response dashboards
Real UAV integration
Live camera-stream processing
Integration with physical drone hardware

🚁 DroneEye
Autonomous aerial monitoring for disaster response.

Detect. Locate. Assess. Respond.

Made for SIH project- SIH26177