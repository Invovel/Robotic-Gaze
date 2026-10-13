# Implementation roadmap

[中文](roadmap.md) | English

Advance on deliverables and acceptance evidence, not assumed calendar progress.

| Stage | Task | Completion criteria | Status |
| --- | --- | --- | --- |
| P01 | Single-axis simulation | Declare the simplified model and units. Apply target steps; save error, control effort, overshoot and settling time. | Not started |
| P02 | Actuator bench | Confirm actuator, driver, power, feedback, limits and emergency stop. Test independently without vision. | Not started |
| P03 | Visual feedback loop | Use simulated or visual targets; evaluate latency, noise, frame drops, target loss and recovery. | Not started |
| P04 | Two-axis extension | Define axes, transforms and calibration. Record coupling; do not directly reuse single-axis gains. | Not started |
| P05 | Control research | Use fixed trajectories to compare delay compensation, filtering and control strategies. Introduce ROS 2 only when system integration needs it. | Not started |

Research extension: Study how observation delay affects stability. Compare methods on the same trajectory and actuator model, then validate again on real hardware.

Update learning notes, results and next steps after each iteration. Preserve failures and their conditions.
