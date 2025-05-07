# TEBot-Navigator  
**ROS-based Autonomous Navigation with Dynamic Obstacle Avoidance**

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
