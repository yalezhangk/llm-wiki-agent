---
title: "RobotAgent"
type: entity
tags: [robot-agent, industrial-robot, health-monitoring, ur5, web-system]
sources: [robot-agent-industrial-robot-health-monitoring-system]
last_updated: 2026-11-18
---
## Summary
[[RobotAgent]] 是一个面向工业机器人（特别是 UR5 机械臂）运行维护场景开发的 Web 化原型系统。它旨在将机械臂运行数据、退化预测模型和健康评估结果集中展示，并串联数据采集、算法训练、模型测试、可视化及维护决策支持流程。

## Key Details
- **目标对象**：主要面向 UR5 机械臂的运行维护场景。
- **系统形态**：Web 化原型系统，提供统一界面展示运行数据、预测模型和健康评估结果。
- **核心流程**：串联采集数据、算法训练、模型测试、结果可视化和维护决策支持。
- **集成模块**：
  - **JLSTM**：误差退化预测。
  - **LLM-Gra**：图增强诊断。
  - **HMM-TCN**：健康评估与预测。
  - **IASTGN**：位姿误差预测。
  - **粒子滤波**：寿命预测。
- **功能覆盖**：精度退化、状态诊断、寿命评估。

## Related
- [[JLSTM]]
- [[LLM-Gra]]
- [[HMM-TCN]]
- [[IASTGN]]
- [[ParticleFiltering]]