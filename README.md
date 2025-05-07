# TEBot-Navigator  
**ROS-based Autonomous Navigation with Dynamic Obstacle Avoidance**

Path Planning Result in Rviz:

<img src="attachments/8938820ad827f7ae8b62ab046f885a26.png" alt="1" style="width: 300px; height: auto;">

⚡ **Highlights**  
- **1150% Speed Boost**: Achieved 6 m/s max velocity through TEB parameter optimization  
- **Sub-10cm Precision**: Enhanced navigation accuracy with adaptive tolerance tuning  
- **Real-Time Optimization**: Sparse matrix-based trajectory solver with 25% faster computation  

🔧 **Tech Stack**  
- **Core**: ROS Noetic | teb_local_planner | Navigation Stack  
- **Simulation**: Gazebo | RViz  
- **Tools**: catkin | g2o optimizer  

✅ **Key Features**  
- Dynamic path replanning with multi-topology parallel planning  
- Velocity/acceleration constraints modeling for differential-drive robots  
- Configurable obstacle inflation layers and costmap strategies  

📊 **Performance Metrics**  
| Metric               | Before | After  | Improvement |
|----------------------|--------|--------|-------------|
| Navigation Time (s)  | 58.2   | 11.7   | 80% ↓       |
| Obstacle Response (ms) | 420   | 82     | 80.5% ↓     |
| CPU Utilization (%)  | 73.5   | 55.2   | 25% ↓       |

📚 **Academic Value**  
- Detailed TEB algorithm analysis with mathematical derivations  
- Step-by-step parameter tuning guide for mobile robots  
- Complete ROS environment deployment tutorials  

🚧 **Tested On**  
`Ubuntu 20.04 LTS` | `ROS Noetic` | `Python3`  

---

## Quick Start
### environment
Windows10 + Ubuntu20.04

### Dependency
1. ros-noetic：
```bash
wget http://fishros.com/install -O fishros && . fishros
```
2. navigation stack：
```bash
sudo apt install ros-noetic-navigation
```
3. teb_local_planner：
```bash
sudo apt install ros-noetic-teb-local-planner
```

### Build
```shell
mkdir -p navigation
cd navigation
mkdir -p src
cd src
catkin_init_workspace
cd ..
catkin_make
source ./devel/setup.bash
```

### Run
```shell
roslaunch navigation run.launch
```

Initial interface after launch: 

<img src="attachments/026f8c1cd68eab020e53d4ac8894a1f0.png" alt="1" style="width: 300px; height: auto;">

