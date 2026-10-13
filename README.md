# Robotic-Gaze · 主动视觉云台

中文 | [English](README.en.md)

如何把视觉误差变成稳定、受限且可恢复的机械运动？

从单轴软件仿真开始，逐步建立带位置反馈的视觉跟随云台，再评估双轴拓展。

状态：2026-10-13，设计起始库。尚未实现新固件、训练模型或开展硬件验收。

## 从这里开始

1. [执行入口](CODEX_START.md)。
2. [设计与边界](docs/design.md)。
3. [实施路线](docs/roadmap.md)。
4. [硬件与基线](hardware/baseline.md)。
5. [学习路径](learning/README.md)。
6. [首个实验](experiments/P01.md)与[记录模板](experiments/template.md)。
7. [设计来源与资料管理](references/origin.md)。

## 独特目标与范围

不重新训练通用视觉模型，不从无刷电机直接跳到整机；不在执行器、驱动、反馈和限位未知时上电。

本库可独立推进，包含自身的设计、学习路径与实验计划。通过测量积累实现证据，未做过的实验不写成成果。
