# Project-driven learning path

[中文](README.md) | English

For each stage, record: question → principle → minimal experiment → observations → interpretation and limits.

## P01: Single-axis simulation

Declare the simplified model and units. Apply target steps; save error, control effort, overshoot and settling time.

Explain inputs, outputs, failure conditions and design choices.

## P02: Actuator bench

Confirm actuator, driver, power, feedback, limits and emergency stop. Test independently without vision.

Explain inputs, outputs, failure conditions and design choices.

## P03: Visual feedback loop

Use simulated or visual targets; evaluate latency, noise, frame drops, target loss and recovery.

Explain inputs, outputs, failure conditions and design choices.

## P04: Two-axis extension

Define axes, transforms and calibration. Record coupling; do not directly reuse single-axis gains.

Explain inputs, outputs, failure conditions and design choices.

## P05: Control research

Use fixed trajectories to compare delay compensation, filtering and control strategies. Introduce ROS 2 only when system integration needs it.

Explain inputs, outputs, failure conditions and design choices.

Add references for the current task rather than collecting a curriculum in advance.
