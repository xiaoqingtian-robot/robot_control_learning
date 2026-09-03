W1 周总结｜Linux + C++ 开发环境 +平衡步兵底盘框架重构

本周基本完成 Linux、GCC/G++、VS Code、Git、CMake 和基础 C++ 开发环境搭建。已经能够在Ubuntu 下创建、编译和运行 C++ 程序，并完成 Git 的 status → add → commit → push 基本工作流。

完成了 robot_control_learning GitHub 仓库，并完成了一个由 CMake 管理的多文件 C++ 项目。

当前 Git 基础操作已经可以使用，但部分命令还不能脱离资料；CMake 能够看懂和修改基础 CMakeLists.txt，但还不能熟练独立编写复杂工程。Linux 命令和 C++ 指针、引用、const 仍需要后续通过项目继续巩固。

第一周的目标主要是建立开发环境和基本工具链，目前已经达到进入下一阶段学习的条件。下一周不再花大量时间学习 Git/CMake，而是在 ROS2 和机器人代码实践中继续使用和巩固。

同时在RM方面，为了备战新赛季，本周开始优化底盘框架，原底盘框架把所有的底盘代码全写在同一个chassis.c文件下，本周完成的有WheelLeg_Chassis.c,WheelLeg_Motor.c,WheelLeg_Kinematics,WheelLeg_Chassis.c提供FreeRTOS的任务接口，WheelLeg_Motor.c底盘相关电机数据统一管理，WheelLeg_Kinematics轮腿底盘五连杆的运动学结算与验证，雅可比矩阵的推算与验证。