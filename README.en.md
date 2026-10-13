# Robotic-Gaze · Active Vision Gimbal

[中文](README.md) | English

How can visual error become stable, bounded and recoverable mechanical motion?

Start with single-axis software simulation, develop a vision-following gimbal with position feedback, then evaluate a two-axis extension.

Status: October 13, 2026 — a design starting point. No new firmware, model training or hardware acceptance has been completed.

## Start here

1. [Next task](CODEX_START.en.md).
2. [Design and scope](docs/design.en.md).
3. [Implementation roadmap](docs/roadmap.en.md).
4. [Hardware and baseline](hardware/baseline.en.md).
5. [Learning path](learning/README.en.md).
6. [First experiment](experiments/P01.en.md) and [record template](experiments/template.en.md).
7. [Design origin and reference management](references/origin.en.md).

## Distinct goal and scope

Do not retrain a general-purpose detector or jump directly from a bare brushless motor to an integrated system. Do not power hardware before the actuator, driver, feedback and limits are defined.

This repository stands on its own, with its own design, learning path and experiments. Build evidence through measurements; do not present unperformed experiments as results.
