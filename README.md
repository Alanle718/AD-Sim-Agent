# Autonomous Driving Simulation Agent (AD-Sim-Agent)

这是一个基于多 Agent 协作的自动驾驶仿真场景自动化生成与测试框架。

## 项目背景
在智能驾驶研发中，覆盖长尾场景（Corner Cases）是提升算法鲁棒性的核心痛点。本项目通过 LLM 驱动的 Agent 协作，实现从“自然语言需求”到“仿真代码生成”再到“安全性能评估”的全链路自动化。

## 核心架构
- **Scenario Planner Agent**: 负责复杂交通逻辑推理，输出标准场景描述。
- **Code Generator Agent**: 将场景逻辑映射到 CARLA / ROS2 的底层 API。
- **Evaluation Agent**: 基于遥测数据（Telemetry）输出多维度的安全评估报告。

## 快速开始
1. 安装依赖: `pip install -r requirements.txt`
2. 运行演示代码: `python ad_simulation_agent.py`

## 未来演进
- 接入真实的 CARLA Python API 物理引擎。
- 支持 C++ 模块的自动注入与编译。
- 集成 ROS2 消息中间件，实现跨节点通信验证。
